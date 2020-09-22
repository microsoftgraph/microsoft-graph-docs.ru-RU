---
title: Тип ресурса authenticationFlowsPolicy
description: 'Представляет конфигурацию политики для интерфейса самостоятельной регистрации на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации. '
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a676014ba6d31ffea08331342504629796f49ec8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034133"
---
# <a name="authenticationflowspolicy-resource-type"></a><span data-ttu-id="7d4b0-103">Тип ресурса authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="7d4b0-103">authenticationFlowsPolicy resource type</span></span>


<span data-ttu-id="7d4b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d4b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d4b0-105">Представляет [конфигурацию политики для интерфейса самостоятельной регистрации](../resources/selfservicesignupauthenticationflowconfiguration.md) на уровне клиента, которая позволяет внешним пользователям запрашивать утверждение регистрации.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-105">Represents the [policy configuration of self-service sign-up experience](../resources/selfservicesignupauthenticationflowconfiguration.md) at a tenant level that lets external users request to sign up for approval.</span></span> <span data-ttu-id="7d4b0-106">Содержит сведения об идентификаторе, отображаемое имя и описание, а также указывает, включена ли самостоятельная регистрация для политики.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-106">It contains information about the ID, display name, and description, and indicates whether self-service sign up is enabled for the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="7d4b0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d4b0-107">Properties</span></span>
|<span data-ttu-id="7d4b0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d4b0-108">Property</span></span>|<span data-ttu-id="7d4b0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7d4b0-109">Type</span></span>|<span data-ttu-id="7d4b0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7d4b0-110">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="7d4b0-111">id</span><span class="sxs-lookup"><span data-stu-id="7d4b0-111">id</span></span>|<span data-ttu-id="7d4b0-112">Строка</span><span class="sxs-lookup"><span data-stu-id="7d4b0-112">String</span></span>| <span data-ttu-id="7d4b0-113">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-113">Inherited property.</span></span> <span data-ttu-id="7d4b0-114">Идентификатор политики потоков проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-114">The ID of the authentication flows policy.</span></span> <span data-ttu-id="7d4b0-115">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-115">Optional.</span></span> <span data-ttu-id="7d4b0-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-116">Read-only.</span></span>
|<span data-ttu-id="7d4b0-117">displayName</span><span class="sxs-lookup"><span data-stu-id="7d4b0-117">displayName</span></span>|<span data-ttu-id="7d4b0-118">Строка</span><span class="sxs-lookup"><span data-stu-id="7d4b0-118">String</span></span>| <span data-ttu-id="7d4b0-119">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-119">Inherited property.</span></span> <span data-ttu-id="7d4b0-120">Понятное для пользователя имя политики.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-120">The human-readable name of the policy.</span></span> <span data-ttu-id="7d4b0-121">Это свойство не является ключевым.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-121">This property is not a key.</span></span> <span data-ttu-id="7d4b0-122">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-122">Optional.</span></span> <span data-ttu-id="7d4b0-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-123">Read-only.</span></span>|
|<span data-ttu-id="7d4b0-124">description</span><span class="sxs-lookup"><span data-stu-id="7d4b0-124">description</span></span>|<span data-ttu-id="7d4b0-125">Строка</span><span class="sxs-lookup"><span data-stu-id="7d4b0-125">String</span></span>|<span data-ttu-id="7d4b0-126">Унаследованное свойство.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-126">Inherited property.</span></span> <span data-ttu-id="7d4b0-127">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-127">A description of the policy.</span></span> <span data-ttu-id="7d4b0-128">Это свойство не является ключевым.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-128">This property is not a key.</span></span> <span data-ttu-id="7d4b0-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-129">Optional.</span></span> <span data-ttu-id="7d4b0-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-130">Read-only.</span></span>|
|<span data-ttu-id="7d4b0-131">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="7d4b0-131">selfServiceSignUp</span></span>|[<span data-ttu-id="7d4b0-132">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d4b0-132">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md) |<span data-ttu-id="7d4b0-133">Содержит параметры [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md), описывающие, включена ли самостоятельная регистрация.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-133">Contains [selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md) settings that convey whether self-service sign-up is enabled or disabled.</span></span> <span data-ttu-id="7d4b0-134">Это свойство не является ключевым.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-134">This property is not a key.</span></span> <span data-ttu-id="7d4b0-135">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-135">Optional.</span></span> <span data-ttu-id="7d4b0-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-136">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7d4b0-137">Связи</span><span class="sxs-lookup"><span data-stu-id="7d4b0-137">Relationships</span></span>
<span data-ttu-id="7d4b0-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d4b0-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7d4b0-139">JSON representation</span></span>
<span data-ttu-id="7d4b0-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d4b0-140">The following is a JSON representation of the resource.</span></span>
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


