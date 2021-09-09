# Лабораторна робота №1

## Хід роботи:

### Добавив свою функцію

    public boolean is_same_birthday(Users user_1,Users user_2) {
        return user_1.dateOfBirth.isEqual(user_2.dateOfBirth);
    }
    
### Створив test функцю 1:
    @Test
    public void whenIsBirthDay_the_same() throws CustomFieldException {
        boolean isBirthday = usersService.is_same_birthday(usersService.getUsers().get(0),usersService.getUsers().get(1));
        assertTrue(isBirthday);
    }
    
### Створив test функцю 2:

    @Test
    public void whenIsBirthDay_not_the_same() throws CustomFieldException {
        boolean isBirthday = usersService.is_same_birthday(usersService.getUsers().get(0),usersService.getUsers().get(1));
        assertFalse(isBirthday);
    }

### Результат при запуску:
!(https://github.com/brunoauditore/NULP_QA/edit/main/lab1/image.png)

