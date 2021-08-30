---
title: selfServiceSignUpAuthenticationFlowConfiguration resource type
description: Представляет конфигурации, связанные с самостоятельной регистрацией.
author: linkhp
ms.localizationpriority: high
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3bab808249ee7417d721e68dbd2a172c71daf593
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696885"
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


