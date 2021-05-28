---
title: тип ресурса сотрудников
description: Объект сотрудника в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: eceea9e1811b61045c03fb8dc5d7710f33158ccc
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52695975"
---
# <a name="employees-resource-type"></a>тип ресурса сотрудников

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сотрудника в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                              | Возвращаемый тип|Описание               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[Получить сотрудников](../api/dynamics-employee-get.md)      |сотрудники  |Получите объект сотрудника.   |
|[Почтовые сотрудники](../api/dynamics-create-employee.md)  |сотрудники  |Создание объекта сотрудника.|
|[Сотрудники исправлений](../api/dynamics-employee-update.md) |сотрудники  |Обновление объекта сотрудника.|
|[Удаление сотрудников](../api/dynamics-employee-delete.md)|нет       |Удаление объекта сотрудника.|

## <a name="properties"></a>Свойства
| Свойство           | Тип   |Описание                                            |
|:-------------------|:-------|:------------------------------------------------------|
|id                  |GUID    |ID сотрудника. Не редактируемый.                         |
|число              |string  |Номер сотрудника. Только для чтения.                        |
|displayName         |string  |Сотрудник, задав имя + фамилию. Только для чтения.           |
|givenName           |string  |Заданное имя сотрудника.                        |
|middleName          |string  |Среднее имя сотрудника.                       |
|surname             |string  |Фамилия сотрудника                            |
|jobTitle;            |string  |Название задания сотрудника                          |
|address             |[NAV. PostalAddress](../resources/dynamics-complextypes.md)|Указывает адрес сотрудника. Этот адрес будет отображаться во всех документах ресурса для сотрудника.|
|phoneNumber         |string  |Указывает телефонный номер сотрудника.             |
|mobilePhone         |string  |Указывает номер мобильного телефона сотрудника.      |
|email               |строка  |Указывает адрес электронной почты сотрудника.                |
|personalEmail       |string  |Указывает личный адрес электронной почты сотрудника.       |
|employmentDate      |date    |Указывает дату начала работы сотрудника в компании.|
|terminationDate     |date    |Указывает дату, когда сотрудник был уволен, например в связи с выходом на пенсию или увольнением.|
|status              |string  |Указывает состояние сотрудника. Возможные значения Active, Inactive или Terminated|
|birthDate           |date    |Указывает дату рождения сотрудника.                |
|изображение             |stream  |Изображение сотрудника. Только для чтения.                       |
|lastModifiedDateTime|datetime|В последний раз сотрудник был изменен. Только для чтения.|  


## <a name="relationships"></a>Связи
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



