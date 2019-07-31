---
title: Тип ресурса Accounts
description: Объект Account в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: cd42177d4886793adedc222cb360a2b3e89faa7e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012690"
---
# <a name="accounts-resource-type"></a>Тип ресурса Accounts
Представляет объект Account в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение учетных записей](../api/dynamics-account-get.md)|см|Получение объекта Accounts.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор учетной записи.|
|число|Строка, максимальный размер 20|Указывает номер финансового счета.|
|displayName|Строка, максимальный размер 50|Указывает имя финансового счета.|
|category|Строка, максимальный размер 20|Указывает категорию финансового счета.|
|Подкатегории|Строка, максимальный размер 80|Указывает подкатегорию категории счетов для финансового счета.|
|заблокированных|boolean|Указывает, что операции не могут быть учтены на финансовом счете. **Значение true** указывает, что учетная запись заблокирована, а Разноска не разрешена.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения учетной записи.|


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
