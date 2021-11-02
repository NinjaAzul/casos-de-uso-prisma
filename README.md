# casos-de-uso-prisma

```
import { PrismaClient } from '@prisma/client'


const prisma = new PrismaClient()



// A `main` function so that you can use async/await
async function main() {
 
  // const resultado = await prisma.user.findMany(); // listALL
  // console.log(resultado);

  //  const resultado = await prisma.user.findMany({
  //    include: {
  //      posts: true,
          // posts: { 
          //   select
          // }
  //    }
  //  }); // listALL where
  // console.log(resultado);

  // const resultado = await prisma.user.create({
  //   data:{
  //     email: "erick",
  //     name: "erick",
  //     posts: {
  //       create: {
  //         title: "post do Luis"
  //       }
  //     }
  //   }
  // })

  //persolalizada
  // const resultado = await prisma.user.findMany({
  //   where: { 
  //     name: {
  //       startsWith: "F"
  //     }
  //   }
  // })

  //Pagination
//   const resultado = await prisma.user.findMany({
//  skip:0,
//  take:1,
//   })


  // const resultado = await prisma.create({
  //   data:{
  //     email:"luist@test.com",
  //   }
  // }); // create
  // console.log(resultado);


  // const resultado = await prisma.update({
  //   data:{
     
  //   },
  //   where:{ id : 1},
  // }); // update
  // console.log(resultado);
  
  //oque faça se não existir este campo
  //UTILIZADO EM SEEDS => 
   // const resultado = await prisma.upsert({
  //   
  //   where:{ id : 1},
  // }); // update
        // create
  // console.log(resultado);

}

main()
  .catch(e => {
    throw e
  })
  .finally(async () => {
    await prisma.$disconnect()
  })

```
