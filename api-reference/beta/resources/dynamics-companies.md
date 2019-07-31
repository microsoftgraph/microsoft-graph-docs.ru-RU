---
title: Тип ресурса "компании"
description: Компания в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 6720a8959ddba79d1face9c91325900c3a35a95c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973732"
---
# <a name="companies-resource-type"></a>Тип ресурса "компании"
Представляет тип ресурса "компании" в Dynamics 365 Business Central. 

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип  |Описание|
|:---------------|:-------------|:----------|
|[Получение компаний](../api/dynamics-companies-get.md)|companies|Получение компании.|

## <a name="properties"></a>Свойства
| Свойство        | Тип |Описание                             |
|:----------------|:-----|:---------------------------------------|
|id               |GUID  |Уникальный идентификатор компании. Только для чтения.|
|name             |string|Указывает компанию.                  |
|displayName      |string|Задает отображаемое имя компании.     |
|Системверсион    |string|Указывает внутреннюю версию компании.|
|Бусинесспрофилеид|string|Указывает идентификатор бизнес-профиля, связанный с компанией.|


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже показано представление компании в формате JSON.

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```


