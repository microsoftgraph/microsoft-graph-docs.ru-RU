---
title: Тип ресурса Accounts
description: Объект Account в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: af6c1eccfc30259f2b86fb5a65b81d95802b67f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505282"
---
# <a name="accounts-resource-type"></a>Тип ресурса Accounts

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|lastModifiedDateTime|datetime|Дата и время последнего изменения учетной записи.|


## <a name="relationships"></a>Связи
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
