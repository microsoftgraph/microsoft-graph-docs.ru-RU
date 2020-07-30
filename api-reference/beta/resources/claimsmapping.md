---
title: Тип ресурса claimsMapping
description: Сопоставление утверждений от маркера с утверждениями, которые распознает и использует Azure Active Directory B2C.
author: namkedia
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fd47f751c71038158761b37721ad8a0d8831eb7d
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510361"
---
# <a name="claimsmapping-resource-type"></a><span data-ttu-id="b4f3d-103">Тип ресурса claimsMapping</span><span class="sxs-lookup"><span data-stu-id="b4f3d-103">claimsMapping resource type</span></span>

<span data-ttu-id="b4f3d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4f3d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b4f3d-105">После того как поставщик настраиваемых удостоверений отправит маркер идентификатора обратно в службу Azure AD B2C, Azure AD B2C сопоставляет утверждения от маркера с утверждениями, которые распознает и использует Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="b4f3d-105">After the custom identity provider sends an ID token back to Azure AD B2C, Azure AD B2C maps the claims from a token to the claims that Azure AD B2C recognizes and uses.</span></span>

## <a name="properties"></a><span data-ttu-id="b4f3d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4f3d-106">Properties</span></span>
|<span data-ttu-id="b4f3d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4f3d-107">Property</span></span>|<span data-ttu-id="b4f3d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b4f3d-108">Type</span></span>|<span data-ttu-id="b4f3d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b4f3d-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="b4f3d-110">userId</span><span class="sxs-lookup"><span data-stu-id="b4f3d-110">userId</span></span>|<span data-ttu-id="b4f3d-111">String</span><span class="sxs-lookup"><span data-stu-id="b4f3d-111">String</span></span>|<span data-ttu-id="b4f3d-112">Утверждение, предоставляющее уникальный идентификатор для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4f3d-112">The claim that provides the unique identifier for the signed-in user.</span></span> <span data-ttu-id="b4f3d-113">Это обязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b4f3d-113">It is a required propoerty.</span></span>|
|<span data-ttu-id="b4f3d-114">displayName</span><span class="sxs-lookup"><span data-stu-id="b4f3d-114">displayName</span></span>|<span data-ttu-id="b4f3d-115">String</span><span class="sxs-lookup"><span data-stu-id="b4f3d-115">String</span></span>|<span data-ttu-id="b4f3d-116">Утверждение, предоставляющее отображаемое или полное имя для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4f3d-116">The claim that provides the display name or full name for the user.</span></span> <span data-ttu-id="b4f3d-117">Это обязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b4f3d-117">It is a required propoerty.</span></span>|
|<span data-ttu-id="b4f3d-118">givenName;</span><span class="sxs-lookup"><span data-stu-id="b4f3d-118">givenName</span></span>|<span data-ttu-id="b4f3d-119">String</span><span class="sxs-lookup"><span data-stu-id="b4f3d-119">String</span></span>|<span data-ttu-id="b4f3d-120">Утверждение, предоставляющее имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4f3d-120">The claim that provides the first name of the user.</span></span>|
|<span data-ttu-id="b4f3d-121">surname</span><span class="sxs-lookup"><span data-stu-id="b4f3d-121">surname</span></span>|<span data-ttu-id="b4f3d-122">String</span><span class="sxs-lookup"><span data-stu-id="b4f3d-122">String</span></span>|<span data-ttu-id="b4f3d-123">Утверждение, предоставляющее фамилию пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4f3d-123">The claim that provides the last name of the user.</span></span>|
|<span data-ttu-id="b4f3d-124">email</span><span class="sxs-lookup"><span data-stu-id="b4f3d-124">email</span></span>|<span data-ttu-id="b4f3d-125">String</span><span class="sxs-lookup"><span data-stu-id="b4f3d-125">String</span></span>|<span data-ttu-id="b4f3d-126">Утверждение, предоставляющее электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4f3d-126">The claim that provides the email address of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4f3d-127">Связи</span><span class="sxs-lookup"><span data-stu-id="b4f3d-127">Relationships</span></span>
<span data-ttu-id="b4f3d-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b4f3d-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4f3d-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b4f3d-129">JSON representation</span></span>
<span data-ttu-id="b4f3d-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4f3d-130">The following is a JSON representation of the resource.</span></span>
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
