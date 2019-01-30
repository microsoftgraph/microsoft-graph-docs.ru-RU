---
title: Тип ресурса implicitGrantSettings
description: Разрешение запроса маркеры, с помощью поток неявных OAuth 2.0 этого веб-приложения. Отдельные свойства доступны для запроса маркеры идентификатор и доступа как часть неявных потока. Чтобы включить неявных поток, по крайней мере одного из следующих свойств необходимо установить значение true.
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642767"
---
# <a name="implicitgrantsettings-resource-type"></a>Тип ресурса implicitGrantSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Разрешение запроса маркеры, с помощью поток неявных OAuth 2.0 этого веб-приложения. Отдельные свойства доступны для запроса маркеры идентификатор и доступа как часть неявных потока. Чтобы включить неявных поток, по крайней мере одного из следующих свойств необходимо установить значение true.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Boolean | Разрешение запроса с помощью поток неявных OAuth 2.0 маркера Идентификации данного веб-приложения.|
|enableAccessTokenIssuance| Boolean | Разрешение запроса маркер доступа с помощью поток неявных OAuth 2.0 этого веб-приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/implicitgrantsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
