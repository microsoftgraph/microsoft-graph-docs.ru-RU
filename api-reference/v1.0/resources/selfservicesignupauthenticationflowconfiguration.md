---
title: selfServiceSignUpAuthenticationFlowConfiguration resource type
description: Представляет конфигурации, связанные с самостоятельной регистрацией.
author: linkhp
ms.localizationpriority: high
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 735803c579f79e9f27f81c53fd9e3fd5ce94e84a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067019"
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
