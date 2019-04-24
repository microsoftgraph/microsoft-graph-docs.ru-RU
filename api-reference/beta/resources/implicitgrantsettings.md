---
title: Тип ресурса ИмплиЦитгрантсеттингс
description: Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0. Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса. Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506228"
---
# <a name="implicitgrantsettings-resource-type"></a>Тип ресурса ИмплиЦитгрантсеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0. Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса. Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
|Енаблеидтокениссуанце| Логический | Указывает, может ли это веб-приложение запрашивать маркер идентификатора с помощью неявного потока OAuth 2,0.|
|Енаблеакцесстокениссуанце| Логический | Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2,0.|

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
