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
# <a name="authenticationsourcefilter-resource-type"></a><span data-ttu-id="d31fa-103">Тип ресурса authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="d31fa-103">authenticationSourceFilter resource type</span></span>

<span data-ttu-id="d31fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d31fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d31fa-105">Фильтрация на основе источника проверки подлинности, используемого для определения того, оценивается ли прослушиватель.</span><span class="sxs-lookup"><span data-stu-id="d31fa-105">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span>

<span data-ttu-id="d31fa-106">Свойство **includeApplications** можно использовать для самостоятельной регистрации в приложении в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d31fa-106">The **includeApplications** property can be used to enable self-service sign up on an application in Azure Active Directory.</span></span> <span data-ttu-id="d31fa-107">Узнайте больше, прочитав нашу документацию по включаю приложения в потоке [самостоятельной регистрации пользователей.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow)</span><span class="sxs-lookup"><span data-stu-id="d31fa-107">Learn more by reading our documentation for [enabling applications in a self-service sign up user flow](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow).</span></span>

## <a name="properties"></a><span data-ttu-id="d31fa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d31fa-108">Properties</span></span>

|<span data-ttu-id="d31fa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d31fa-109">Property</span></span>|<span data-ttu-id="d31fa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d31fa-110">Type</span></span>|<span data-ttu-id="d31fa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d31fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d31fa-112">includeApplications</span><span class="sxs-lookup"><span data-stu-id="d31fa-112">includeApplications</span></span>|<span data-ttu-id="d31fa-113">Набор строк</span><span class="sxs-lookup"><span data-stu-id="d31fa-113">String collection</span></span>|<span data-ttu-id="d31fa-114">Приложения, которые необходимо включить для оценки [authenticationListener.](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="d31fa-114">Applications to include for evaluation of the [authenticationListener](../resources/authenticationlistener.md).</span></span> <span data-ttu-id="d31fa-115">Эти приложения запускают связанное действие при его применении в качестве клиентского приложения в потоке проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d31fa-115">These applications trigger the associated action when used as the client application in the authentication flow.</span></span> <span data-ttu-id="d31fa-116">Identifer приложения — это ид клиента приложения.</span><span class="sxs-lookup"><span data-stu-id="d31fa-116">The application identifer is the application's client id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d31fa-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="d31fa-117">Relationships</span></span>

<span data-ttu-id="d31fa-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d31fa-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d31fa-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d31fa-119">JSON representation</span></span>

<span data-ttu-id="d31fa-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d31fa-120">The following is a JSON representation of the resource.</span></span>
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
