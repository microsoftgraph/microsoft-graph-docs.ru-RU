---
title: Тип ресурса "компании"
description: Компания в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: f1faca36af25bc8cb3e9019e0dc5b4460991e70d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543110"
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
|id               |Глобальный уникальный идентификатор (GUID)  |Уникальный идентификатор компании. Только для чтения.|
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


