---
title: Тип ресурса authenticationFlowsPolicy
description: 'Представляет конфигурацию политики для интерфейса самостоятельной регистрации на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации. '
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cc7f6261e4db4b908d6ab3e0ab3c41504ce8462b
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232111"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="d5e89-103">Тип ресурса authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="d5e89-103">authenticationFlowsPolicy resource type</span></span>


<span data-ttu-id="d5e89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5e89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5e89-105">Представляет [конфигурацию политики для интерфейса самостоятельной регистрации](../resources/selfservicesignupauthenticationflowconfiguration.md) на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации.</span><span class="sxs-lookup"><span data-stu-id="d5e89-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="d5e89-106">Содержит сведения об идентификаторе, отображаемое имя и описание, а также указывает, включена ли самостоятельная регистрация для политики.</span><span class="sxs-lookup"><span data-stu-id="d5e89-106">It contains information about the ID, display name, and description, and indicates whether self-service sign up is enabled for the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="d5e89-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5e89-107">Properties</span></span>
|<span data-ttu-id="d5e89-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5e89-108">Property</span></span>|<span data-ttu-id="d5e89-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d5e89-109">Type</span></span>|<span data-ttu-id="d5e89-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d5e89-110">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="d5e89-111">id</span><span class="sxs-lookup"><span data-stu-id="d5e89-111">id</span></span>|<span data-ttu-id="d5e89-112">Строка</span><span class="sxs-lookup"><span data-stu-id="d5e89-112">String</span></span>| <span data-ttu-id="d5e89-113">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="d5e89-113">Inherited property.</span></span> <span data-ttu-id="d5e89-114">Идентификатор политики потоков проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d5e89-114">The ID of the authentication flows policy.</span></span> <span data-ttu-id="d5e89-115">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d5e89-115">Optional.</span></span> <span data-ttu-id="d5e89-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5e89-116">Read-only.</span></span>
|<span data-ttu-id="d5e89-117">displayName</span><span class="sxs-lookup"><span data-stu-id="d5e89-117">displayName</span></span>|<span data-ttu-id="d5e89-118">Строка</span><span class="sxs-lookup"><span data-stu-id="d5e89-118">String</span></span>| <span data-ttu-id="d5e89-119">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="d5e89-119">Inherited property.</span></span> <span data-ttu-id="d5e89-120">Понятное для пользователя имя политики.</span><span class="sxs-lookup"><span data-stu-id="d5e89-120">The human-readable name of the policy.</span></span> <span data-ttu-id="d5e89-121">Это свойство не является ключевым.</span><span class="sxs-lookup"><span data-stu-id="d5e89-121">This property is not a key.</span></span> <span data-ttu-id="d5e89-122">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d5e89-122">Optional.</span></span> <span data-ttu-id="d5e89-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5e89-123">Read-only.</span></span>|
|<span data-ttu-id="d5e89-124">description</span><span class="sxs-lookup"><span data-stu-id="d5e89-124">description</span></span>|<span data-ttu-id="d5e89-125">Строка</span><span class="sxs-lookup"><span data-stu-id="d5e89-125">String</span></span>|<span data-ttu-id="d5e89-126">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="d5e89-126">Inherited property.</span></span> <span data-ttu-id="d5e89-127">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="d5e89-127">A description of the policy.</span></span> <span data-ttu-id="d5e89-128">Это свойство не является ключевым.</span><span class="sxs-lookup"><span data-stu-id="d5e89-128">This property is not a key.</span></span> <span data-ttu-id="d5e89-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d5e89-129">Optional.</span></span> <span data-ttu-id="d5e89-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5e89-130">Read-only.</span></span>|
|<span data-ttu-id="d5e89-131">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="d5e89-131">selfServiceSignUp</span></span>|[<span data-ttu-id="d5e89-132">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5e89-132">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="d5e89-133">Содержит параметры [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md), описывающие, включена ли самостоятельная регистрация.</span><span class="sxs-lookup"><span data-stu-id="d5e89-133">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="d5e89-134">Это свойство не является ключевым.</span><span class="sxs-lookup"><span data-stu-id="d5e89-134">This property is not a key.</span></span> <span data-ttu-id="d5e89-135">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d5e89-135">Optional.</span></span> <span data-ttu-id="d5e89-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5e89-136">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d5e89-137">Связи</span><span class="sxs-lookup"><span data-stu-id="d5e89-137">Relationships</span></span>
<span data-ttu-id="d5e89-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d5e89-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5e89-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d5e89-139">JSON representation</span></span>
<span data-ttu-id="d5e89-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5e89-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy",
  "openType": false
}
-->

``` json
{
   "id":"String (identifier)",
   "displayName":"String",
   "description":"String",
   "selfServiceSignUp":{
      "@odata.type":"#microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
   }
}
```


