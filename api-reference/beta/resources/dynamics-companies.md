---
title: Тип ресурса "компании"
description: Компания в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 3fedbd9407a4124c38a6ff08a95dbf4cd22c9fe1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081766"
---
# <a name="companies-resource-type"></a>Тип ресурса "компании"

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|системверсион    |string|Указывает внутреннюю версию компании.|
|бусинесспрофилеид|string|Указывает идентификатор бизнес-профиля, связанный с компанией.|


## <a name="relationships"></a>Связи
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




