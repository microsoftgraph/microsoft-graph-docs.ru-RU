---
title: Тип ресурса claimsMapping
description: Сопоставление утверждений от маркера с утверждениями, которые распознает и использует Azure Active Directory B2C.
author: namkedia
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1863c6bf6f28e0e8ae8a3d1133330337a7420c0a
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761844"
---
# <a name="claimsmapping-resource-type"></a><span data-ttu-id="e5d3b-103">Тип ресурса claimsMapping</span><span class="sxs-lookup"><span data-stu-id="e5d3b-103">claimsMapping resource type</span></span>

<span data-ttu-id="e5d3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5d3b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5d3b-105">После того как поставщик настраиваемых удостоверений отправит маркер идентификатора обратно в службу Azure AD B2C, Azure AD B2C сопоставляет утверждения от маркера с утверждениями, которые распознает и использует Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="e5d3b-105">After the custom identity provider sends an ID token back to Azure AD B2C, Azure AD B2C maps the claims from a token to the claims that Azure AD B2C recognizes and uses.</span></span>

## <a name="properties"></a><span data-ttu-id="e5d3b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5d3b-106">Properties</span></span>
|<span data-ttu-id="e5d3b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5d3b-107">Property</span></span>|<span data-ttu-id="e5d3b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e5d3b-108">Type</span></span>|<span data-ttu-id="e5d3b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e5d3b-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="e5d3b-110">userId</span><span class="sxs-lookup"><span data-stu-id="e5d3b-110">userId</span></span>|<span data-ttu-id="e5d3b-111">String</span><span class="sxs-lookup"><span data-stu-id="e5d3b-111">String</span></span>|<span data-ttu-id="e5d3b-112">Утверждение, предоставляющее уникальный идентификатор для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="e5d3b-112">The claim that provides the unique identifier for the signed-in user.</span></span> <span data-ttu-id="e5d3b-113">Это обязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="e5d3b-113">It is a required propoerty.</span></span>|
|<span data-ttu-id="e5d3b-114">displayName</span><span class="sxs-lookup"><span data-stu-id="e5d3b-114">displayName</span></span>|<span data-ttu-id="e5d3b-115">String</span><span class="sxs-lookup"><span data-stu-id="e5d3b-115">String</span></span>|<span data-ttu-id="e5d3b-116">Утверждение, предоставляющее отображаемое или полное имя для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e5d3b-116">The claim that provides the display name or full name for the user.</span></span> <span data-ttu-id="e5d3b-117">Это обязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="e5d3b-117">It is a required propoerty.</span></span>|
|<span data-ttu-id="e5d3b-118">givenName;</span><span class="sxs-lookup"><span data-stu-id="e5d3b-118">givenName</span></span>|<span data-ttu-id="e5d3b-119">String</span><span class="sxs-lookup"><span data-stu-id="e5d3b-119">String</span></span>|<span data-ttu-id="e5d3b-120">Утверждение, предоставляющее имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="e5d3b-120">The claim that provides the first name of the user.</span></span>|
|<span data-ttu-id="e5d3b-121">surname</span><span class="sxs-lookup"><span data-stu-id="e5d3b-121">surname</span></span>|<span data-ttu-id="e5d3b-122">String</span><span class="sxs-lookup"><span data-stu-id="e5d3b-122">String</span></span>|<span data-ttu-id="e5d3b-123">Утверждение, предоставляющее фамилию пользователя.</span><span class="sxs-lookup"><span data-stu-id="e5d3b-123">The claim that provides the last name of the user.</span></span>|
|<span data-ttu-id="e5d3b-124">email</span><span class="sxs-lookup"><span data-stu-id="e5d3b-124">email</span></span>|<span data-ttu-id="e5d3b-125">String</span><span class="sxs-lookup"><span data-stu-id="e5d3b-125">String</span></span>|<span data-ttu-id="e5d3b-126">Утверждение, предоставляющее электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="e5d3b-126">The claim that provides the email address of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5d3b-127">Связи</span><span class="sxs-lookup"><span data-stu-id="e5d3b-127">Relationships</span></span>
<span data-ttu-id="e5d3b-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5d3b-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5d3b-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e5d3b-129">JSON representation</span></span>
<span data-ttu-id="e5d3b-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5d3b-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.claimsMapping"
}
-->

``` json
{
  "userId": "String",
  "givenName": "String",
  "surname": "String",
  "email": "String",
  "displayName": "String"
  }
```


