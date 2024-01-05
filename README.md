# Asynchronous-Tasks-
Python Code for Asynchronous Tasks with asyncio
import asyncio

async def task1():
    await asyncio.sleep(1)
    print('Task 1 completed')

async def task2():
    await asyncio.sleep(2)
    print('Task 2 completed')

async def main():
    await asyncio.gather(task1(), task2())

asyncio.run(main())
