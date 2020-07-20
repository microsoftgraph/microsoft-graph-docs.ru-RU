---
title: Тип ресурса Аусентикатионфловсполици
description: 'Представляет конфигурацию политики взаимодействия с самостоятельной регистрацией на уровне клиента, с помощью которой внешние пользователи могут подписаться на утверждение. '
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 263b92c081545fc3ce337d25b4813d85fe034940
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556462"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="a5817-103">Тип ресурса Аусентикатионфловсполици</span><span class="sxs-lookup"><span data-stu-id="a5817-103">authenticationFlowsPolicy resource type</span></span>


<span data-ttu-id="a5817-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5817-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5817-105">Представляет [конфигурацию политики взаимодействия с самостоятельной регистрацией](../resources/selfservicesignupauthenticationflowconfiguration.md) на уровне клиента, с помощью которой внешние пользователи могут подписаться на утверждение.</span><span class="sxs-lookup"><span data-stu-id="a5817-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="a5817-106">Он содержит сведения об ИДЕНТИФИКАТОРе, отображаемое имя и описание, а также указывает, включена ли функция регистрации самостоятельных служб для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a5817-106">It contains information about the ID, display name, and description, and indicates whether self-service sign up is enabled for the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="a5817-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5817-107">Properties</span></span>
|<span data-ttu-id="a5817-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5817-108">Property</span></span>|<span data-ttu-id="a5817-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a5817-109">Type</span></span>|<span data-ttu-id="a5817-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a5817-110">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="a5817-111">id</span><span class="sxs-lookup"><span data-stu-id="a5817-111">id</span></span>|<span data-ttu-id="a5817-112">String</span><span class="sxs-lookup"><span data-stu-id="a5817-112">String</span></span>| <span data-ttu-id="a5817-113">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="a5817-113">Inherited property.</span></span> <span data-ttu-id="a5817-114">Идентификатор политики потоков проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="a5817-114">The ID of the authentication flows policy.</span></span> <span data-ttu-id="a5817-115">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a5817-115">Optional.</span></span> <span data-ttu-id="a5817-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5817-116">Read-only.</span></span>
|<span data-ttu-id="a5817-117">displayName</span><span class="sxs-lookup"><span data-stu-id="a5817-117">displayName</span></span>|<span data-ttu-id="a5817-118">Строка</span><span class="sxs-lookup"><span data-stu-id="a5817-118">String</span></span>| <span data-ttu-id="a5817-119">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="a5817-119">Inherited property.</span></span> <span data-ttu-id="a5817-120">Понятное для человека имя политики.</span><span class="sxs-lookup"><span data-stu-id="a5817-120">The human-readable name of the policy.</span></span> <span data-ttu-id="a5817-121">Это свойство не является ключом.</span><span class="sxs-lookup"><span data-stu-id="a5817-121">This property is not a key.</span></span> <span data-ttu-id="a5817-122">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a5817-122">Optional.</span></span> <span data-ttu-id="a5817-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5817-123">Read-only.</span></span>|
|<span data-ttu-id="a5817-124">description</span><span class="sxs-lookup"><span data-stu-id="a5817-124">description</span></span>|<span data-ttu-id="a5817-125">String</span><span class="sxs-lookup"><span data-stu-id="a5817-125">String</span></span>|<span data-ttu-id="a5817-126">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="a5817-126">Inherited property.</span></span> <span data-ttu-id="a5817-127">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="a5817-127">A description of the policy.</span></span> <span data-ttu-id="a5817-128">Это свойство не является ключом.</span><span class="sxs-lookup"><span data-stu-id="a5817-128">This property is not a key.</span></span> <span data-ttu-id="a5817-129">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a5817-129">Optional.</span></span> <span data-ttu-id="a5817-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5817-130">Read-only.</span></span>|
|<span data-ttu-id="a5817-131">селфсервицесигнуп</span><span class="sxs-lookup"><span data-stu-id="a5817-131">selfServiceSignUp</span></span>|[<span data-ttu-id="a5817-132">селфсервицесигнупаусентикатионфловконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a5817-132">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="a5817-133">Содержит параметры [селфсервицесигнупаусентикатионфловконфигуратион](../resources/selfservicesignupauthenticationflowconfiguration.md) , которые сообщают, включена или отключена самостоятельная регистрация.</span><span class="sxs-lookup"><span data-stu-id="a5817-133">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="a5817-134">Это свойство не является ключом.</span><span class="sxs-lookup"><span data-stu-id="a5817-134">This property is not a key.</span></span> <span data-ttu-id="a5817-135">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a5817-135">Optional.</span></span> <span data-ttu-id="a5817-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5817-136">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a5817-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="a5817-137">Relationships</span></span>
<span data-ttu-id="a5817-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a5817-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5817-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a5817-139">JSON representation</span></span>
<span data-ttu-id="a5817-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5817-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "selfServiceSignUp": {
    "@odata.type": "#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
  },
}
```
