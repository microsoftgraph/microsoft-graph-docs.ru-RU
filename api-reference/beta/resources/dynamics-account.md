---
title: Тип ресурса Accounts
description: Объект Account в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507576"
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
|number|Строка, максимальный размер 20|Указывает номер финансового счета.|
|displayName|Строка, максимальный размер 50|Указывает имя финансового счета.|
|category|Строка, максимальный размер 20|Указывает категорию финансового счета.|
|Подкатегории|Строка, максимальный размер 80|Указывает подкатегорию категории счетов для финансового счета.|
|заблокированных|логический|Указывает, что операции не могут быть учтены на финансовом счете. **Значение true** указывает, что учетная запись заблокирована, а Разноска не разрешена.|
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
