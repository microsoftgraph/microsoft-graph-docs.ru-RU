---
title: Тип ресурса authenticationSourceFilter
description: Фильтр на основе источника проверки подлинности, который используется для определения того, выполняется ли прослушиватель.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4736be415faab65c6ce3b572a1273a73c707ee43
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128633"
---
# <a name="authenticationsourcefilter-resource-type"></a>Тип ресурса authenticationSourceFilter

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Фильтрация на основе источника проверки подлинности, используемого для определения того, оценивается ли прослушиватель.

Свойство **includeApplications** можно использовать для самостоятельной регистрации в приложении в Azure Active Directory. Узнайте больше, прочитав нашу документацию по предоставлению приложениям возможности самостоятельной [регистрации пользовательского потока.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow)

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|includeApplications|Коллекция объектов string|Приложения, которые необходимо включить для оценки [authenticationListener.](../resources/authenticationlistener.md) Эти приложения запускают связанное действие при его применении в качестве клиентского приложения в потоке проверки подлинности. Identifer приложения — это ид клиента приложения.|

## <a name="relationships"></a>Связи

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
