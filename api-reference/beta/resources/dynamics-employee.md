---
title: Тип ресурса Employees
description: Объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d404a1ede257f3a31371dba31c37ff329452fccd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071341"
---
# <a name="employees-resource-type"></a>Тип ресурса Employees

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|id                  |GUID    |Идентификатор сотрудника. Не редактируемые.                         |
|число              |string  |Номер сотрудника. Только для чтения.                        |
|displayName         |string  |Сотрудник givenName + фамилия. Только для чтения.           |
|givenName;           |string  |Заданное имя сотрудника.                        |
|middleName          |string  |Отчество сотрудника.                       |
|surname             |string  |Фамилия сотрудника                            |
|jobTitle;            |string  |Полное имя сотрудника                          |
|address             |[Навигационная. посталаддресс](../resources/dynamics-complextypes.md)|Указывает адрес сотрудника. Этот адрес будет отображаться во всех документах ресурсов для сотрудника.|
|phoneNumber         |string  |Указывает номер телефона сотрудника.             |
|mobilePhone         |string  |Указывает номер мобильного телефона сотрудника.      |
|email               |строка  |Указывает адрес электронной почты сотрудника.                |
|персоналемаил       |string  |Указывает личный адрес электронной почты сотрудника.       |
|емплойментдате      |date    |Указывает дату начала работы сотрудника в компании.|
|терминатиондате     |date    |Указывает дату увольнения сотрудника, например из-за увольнения или увольнения.|
|status              |string  |Указывает состояние сотрудника. Возможные значения: активные, неактивные или прерванные|
|birthDate           |date    |Указывает дату рождения сотрудника.                |
|графические             |stream  |Фотография сотрудника. Только для чтения.                       |
|lastModifiedDateTime|datetime|Дата и время последнего изменения сотрудника. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

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



