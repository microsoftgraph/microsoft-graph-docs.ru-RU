---
title: Тип ресурса "компании"
description: Компания в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: f1faca36af25bc8cb3e9019e0dc5b4460991e70d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365684"
---
# <a name="companies-resource-type"></a>Тип ресурса "компании"
Представляет тип ресурса "компании" в Dynamics 365 Business Central. 

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип  |Описание|
|:---------------|:-------------|:----------|
|[Получение компаний](../api/dynamics-companies-get.md)|коммуналь|Получение компании.|

## <a name="properties"></a>Свойства
| Свойство        | Тип |Описание                             |
|:----------------|:-----|:---------------------------------------|
|id               |GUID  |Уникальный идентификатор компании. Только для чтения.|
|name             |string|Указывает компанию.                  |
|displayName      |строка|Задает отображаемое имя компании.     |
|Системверсион    |строка|Указывает внутреннюю версию компании.|
|Бусинесспрофилеид|строка|Указывает идентификатор бизнес-профиля, связанный с компанией.|


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

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


