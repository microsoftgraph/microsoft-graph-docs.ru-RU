---
title: Тип ресурса Employees
description: Объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 865da0c1e1256e2ba2a25902e37a00da9081eedf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543065"
---
# <a name="employees-resource-type"></a>Тип ресурса Employees
Представляет сотрудника в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                              | Возвращаемый тип|Описание               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[Получение сотрудников](../api/dynamics-employee-get.md)      |сотрудников  |Получение объекта Employee.   |
|[Учет сотрудников](../api/dynamics-create-employee.md)  |сотрудников  |Создание объекта Employee.|
|[Обновление сотрудников](../api/dynamics-employee-update.md) |сотрудников  |Обновление объекта Employee.|
|[Удаление сотрудников](../api/dynamics-employee-delete.md)|Нет       |Удаление объекта Employee.|

## <a name="properties"></a>Свойства
| Свойство           | Тип   |Описание                                            |
|:-------------------|:-------|:------------------------------------------------------|
|id                  |Глобальный уникальный идентификатор (GUID)    |Идентификатор сотрудника. Не редактируемые.                         |
|число              |string  |Номер сотрудника. Только для чтения.                        |
|displayName         |string  |Сотрудник givenName + фамилия. Только для чтения.           |
|givenName           |string  |Заданное имя сотрудника.                        |
|middleName          |string  |Отчество сотрудника.                       |
|surname             |string  |Фамилия сотрудника                            |
|jobTitle            |string  |Полное имя сотрудника                          |
|address             |[Навигационная. Посталаддресс](../resources/dynamics-complextypes.md)|Указывает адрес сотрудника. Этот адрес будет отображаться во всех документах ресурсов для сотрудника.|
|phoneNumber         |string  |Указывает номер телефона сотрудника.             |
|mobilePhone         |string  |Указывает номер мобильного телефона сотрудника.      |
|email               |string  |Указывает адрес электронной почты сотрудника.                |
|Персоналемаил       |string  |Указывает личный адрес электронной почты сотрудника.       |
|Емплойментдате      |дата    |Указывает дату начала работы сотрудника в компании.|
|Терминатиондате     |дата    |Указывает дату увольнения сотрудника, например из-за увольнения или увольнения.|
|status              |string  |Указывает состояние сотрудника. Возможные значения: активные, неАктивные или прерванные|
|birthDate           |дата    |Указывает дату рождения сотрудника.                |
|графические             |stream  |Фотография сотрудника. Только для чтения.                       |
|lastModifiedDateTime|отличным|Дата и время последнего изменения сотрудника. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "givenName": "string",
    "middleName": "string",
    "surname": "string",
    "jobTitle": "string",
    "address": "NAV.PostalAddress",
    "phoneNumber": "string",
    "mobilePhone": "string",
    "email": "string",
    "personalEmail": "string",
    "employmentDate": "date",
    "terminationDate": "date",
    "status": "string",
    "birthDate": "date",
    "picture": "stream",
    "lastModifiedDateTime": "datetime"
}

```

