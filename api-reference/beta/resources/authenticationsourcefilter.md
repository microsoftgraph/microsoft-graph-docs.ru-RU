---
title: Тип ресурса authenticationSourceFilter
description: Фильтр на основе источника проверки подлинности, который используется для определения того, выполняется ли прослушиватель.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0fcbeb3296b6b0dece1b69cedf26d600c240d43d
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720443"
---
# <a name="authenticationsourcefilter-resource-type"></a>Тип ресурса authenticationSourceFilter

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Фильтрация на основе источника проверки подлинности, используемого для определения того, оценивается ли прослушиватель.

Свойство **includeApplications** можно использовать для самостоятельной регистрации в приложении в Azure Active Directory. Узнайте больше, прочитав нашу документацию по включаю приложения в потоке [самостоятельной регистрации пользователей.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow)

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|includeApplications|Набор строк|Приложения, которые необходимо включить для оценки [authenticationListener.](../resources/authenticationlistener.md) Эти приложения запускают связанное действие при его применении в качестве клиентского приложения в потоке проверки подлинности. Identifer приложения — это ид клиента приложения.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationSourceFilter"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationSourceFilter",
  "includeApplications": [
    "String"
  ]
}
```
