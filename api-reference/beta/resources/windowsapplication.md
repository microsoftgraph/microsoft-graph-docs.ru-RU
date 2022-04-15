---
title: Тип ресурса windowsApplication
description: Представляет параметры для приложений, работающих Windows Microsoft и опубликованных в магазине Microsoft Store или Xbox.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: aricrowe57
ms.openlocfilehash: 9472a8c39a9ddeb7ed7a3857c5bba11c8435d44c
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848685"
---
# <a name="windowsapplication-resource-type"></a>Тип ресурса windowsApplication

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры для приложений, работающих Windows Microsoft и опубликованных в магазине Microsoft Store или Xbox.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| packageSid | String | Идентификатор безопасности пакета, назначенный корпорацией Майкрософт приложению. Необязательно. Только для чтения. |
| redirectUris | Коллекция String | Указывает URL-адреса, куда отправляются маркеры пользователя для входа, или URI перенаправления, в которые отправляются коды авторизации OAuth 2.0 и маркеры доступа. Доступно только для приложений, поддерживающих `PersonalMicrosoftAccount` **signInAudience**. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.windowsApplication"
}-->

```json
{
  "packageSid": "String",
  "redirectUris": ["String"]
}

```
