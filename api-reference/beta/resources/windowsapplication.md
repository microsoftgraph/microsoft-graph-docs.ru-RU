---
title: тип ресурса windowsApplication
description: Представляет параметры приложений под управлением Microsoft Windows и опубликованных в Microsoft Store или магазине игр Xbox.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: aricrowe57
ms.openlocfilehash: 7caedf0d8f8cda38129cfc108a2e4dc7ce609279
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339224"
---
# <a name="webapplication-resource-type"></a>Тип ресурса webApplication

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры приложений под управлением Microsoft Windows и опубликованных в Microsoft Store или магазине игр Xbox.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| packageSid | Строка | Идентификатор безопасности пакета, назначенный корпорацией Майкрософт приложению. Необязательно. Только для чтения. |
| redirectUris | Коллекция объектов string | Указывает URL-адреса, куда отправляются маркеры пользователей для регистрации или URL-адреса перенаправления, куда отправляются коды авторизации OAuth 2.0 и маркеры доступа. Доступно только для приложений, поддерживаюных `PersonalMicrosoftAccount` **signInAudience**. |

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