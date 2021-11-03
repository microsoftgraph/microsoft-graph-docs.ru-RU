---
title: тип ресурса appManagementConfiguration
description: Объект конфигурации управления приложениями, содержащий свойства, которые можно настроить, чтобы включить различные ограничения для приложений и основных служб.
author: madansr7
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c87918a001e5ede8a521f7ff666f902ba9d28b54
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695619"
---
# <a name="appmanagementconfiguration-resource-type"></a>тип ресурса appManagementConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект конфигурации управления приложениями, содержащий свойства, которые можно настроить, чтобы включить различные ограничения для приложений и основных служб.

## <a name="properties"></a>Свойства

| Свойство            | Тип                                                                  | Описание                                                                                       |
| :------------------ | :-------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------ |
| passwordCredentials | [коллекция passwordCredentialConfiguration](passwordCredentialConfiguration.md) | Набор параметров ограничений паролей, которые будут применены к приложению или директору службы. |
| keyCredentials | [коллекция keyCredentialConfiguration](keyCredentialConfiguration.md) | Коллекция параметров ограничений keyCredential, которые будут применены к приложению или директору службы. |

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
   ],
   "keyCredentials": [
    {
      "@odata.type": "microsoft.graph.keyCredentialConfiguration"
    }
   ]
}
```
