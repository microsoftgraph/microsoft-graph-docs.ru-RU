---
title: Тип ресурса Селфсервицесигнупаусентикатионфловконфигуратион
description: Представляет конфигурации, связанные с регистрацией самостоятельной службы.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8c75b3a90a7e9de01234bb53ed8346c40eef932f
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556449"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a>Тип ресурса Селфсервицесигнупаусентикатионфловконфигуратион


Пространство имен: microsoft.graph

Представляет конфигурации, связанные с самостоятельным входом.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:-------|:---|:----------|
|isEnabled|Boolean|Указывает, включен или отключен процесс самостоятельной регистрации для самостоятельных служб. Значение по умолчанию — `false`. Это свойство не является ключом. Обязательный элемент. |

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
