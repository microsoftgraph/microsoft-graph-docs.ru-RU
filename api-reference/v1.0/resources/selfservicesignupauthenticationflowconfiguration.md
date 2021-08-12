---
title: selfServiceSignUpAuthenticationFlowConfiguration resource type
description: Представляет конфигурации, связанные с самостоятельной регистрацией.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 96800f7b3ef2509cf52a302409b03cfc2d3fd62dee864da99ecf6ecf8e3bde7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126286"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a>selfServiceSignUpAuthenticationFlowConfiguration resource type

Пространство имен: microsoft.graph

Представляет конфигурации, связанные с самостоятельной регистрацией.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:-------|:---|:----------|
|isEnabled|Boolean|Указывает, включена или выключена ли самостоятельная регистрация. Значение по умолчанию — `false`. Это свойство не является ключевым. Обязательный. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
}
-->

``` json
{
  "isEnabled": "Boolean"
}
```
