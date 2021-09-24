---
title: тип ресурса authenticationSourceFilter
description: Фильтр на основе источника проверки подлинности, который используется для определения того, выполняется ли прослушиватель или нет.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 53f765f998dffdce5dcfd549177ebd1250cf013f
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508014"
---
# <a name="authenticationsourcefilter-resource-type"></a>тип ресурса authenticationSourceFilter

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Фильтр на основе источника проверки подлинности, который используется для определения оценки прослушиваемого.

Свойство **includeApplications** можно использовать для того, чтобы включить самообслуживление для регистрации в приложении в Azure Active Directory. Узнайте больше, прочитав документацию о включающих приложениях в самообслуживной [регистрации потока пользователей.](/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow)

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|includeApplications|Коллекция объектов string|Приложения, которые необходимо включить для оценки [проверки подлинностиListener](../resources/authenticationlistener.md). Эти приложения вызывают связанное действие при его применении в качестве клиентского приложения в потоке проверки подлинности. Identifer приложения — это клиентский id приложения.|

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
