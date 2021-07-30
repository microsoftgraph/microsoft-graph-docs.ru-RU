---
title: тип ресурса appManagementConfiguration
description: Объект конфигурации управления приложениями, содержащий свойства, которые можно настроить, чтобы включить различные ограничения для приложений и основных служб.
author: madansr7
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fb8d64a746b9863116f9149a435afe9ac3998c7c
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660480"
---
# <a name="appmanagementconfiguration-resource-type"></a>тип ресурса appManagementConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект конфигурации управления приложениями, содержащий свойства, которые можно настроить, чтобы включить различные ограничения для приложений и основных служб.

## <a name="properties"></a>Свойства

| Свойство            | Тип                                                                  | Описание                                                                                       |
| :------------------ | :-------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------ |
| passwordCredentials | [коллекция passwordCredentialConfiguration](passwordCredentialConfiguration.md) | Коллекция параметров ограничений паролей, которые будут применены к основному приложению или службе |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appManagementConfiguration"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.appManagementConfiguration",
  "passwordCredentials": [
    {
      "@odata.type": "microsoft.graph.passwordCredentialConfiguration"
    }
   ]
}
```
