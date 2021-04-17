---
title: selfServiceSignUpAuthenticationFlowConfiguration resource type
description: Представляет конфигурации, связанные с самостоятельной регистрацией.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a235c9e9869b3e0b0c36b0369ae6163083b3cf20
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883314"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a>selfServiceSignUpAuthenticationFlowConfiguration resource type

Пространство имен: microsoft.graph

Представляет конфигурации, связанные с самостоятельной регистрацией.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:-------|:---|:----------|
|isEnabled|Boolean|Указывает, включена или выключена ли самостоятельная регистрация. Значение по умолчанию — `false`. Это свойство не является ключевым. Обязательный. |

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
