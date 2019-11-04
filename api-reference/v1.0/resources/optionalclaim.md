---
title: Тип ресурса Оптионалклаим
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: sureshja
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d580809ab5046720730578713e90588c6f6ec49a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939020"
---
# <a name="optionalclaim-resource-type"></a><span data-ttu-id="95c81-103">Тип ресурса Оптионалклаим</span><span class="sxs-lookup"><span data-stu-id="95c81-103">optionalClaim resource type</span></span>

<span data-ttu-id="95c81-104">Содержит необязательное утверждение, связанное с [приложением](application.md)</span><span class="sxs-lookup"><span data-stu-id="95c81-104">Contains an optional claim associated with an [application](application.md)</span></span> <!-- or a service principal --><span data-ttu-id="95c81-105">.</span><span class="sxs-lookup"><span data-stu-id="95c81-105"></span></span> <span data-ttu-id="95c81-106">Свойства `idToken`, `accessToken`и `saml2Token` , в ресурсе [оптионалклаимс](optionalclaims.md) , представляют собой коллекцию **оптионалклаим**.</span><span class="sxs-lookup"><span data-stu-id="95c81-106">The `idToken`, `accessToken`, and `saml2Token` properties of the [optionalClaims](optionalclaims.md) resource is a collection of **optionalClaim**.</span></span> <span data-ttu-id="95c81-107">Если это поддерживается определенным утверждением, вы также можете изменить поведение Оптионалклаим с помощью `additionalProperties` свойства.</span><span class="sxs-lookup"><span data-stu-id="95c81-107">If supported by a specific claim, you can also modify the behavior of the optionalClaim using the `additionalProperties` property.</span></span> 

<span data-ttu-id="95c81-108">Дополнительные сведения см. [в статье предоставление дополнительных утверждений для приложения Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-optional-claims) .</span><span class="sxs-lookup"><span data-stu-id="95c81-108">See [provide optional claims to your Azure AD app](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="95c81-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="95c81-109">Properties</span></span>

| <span data-ttu-id="95c81-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="95c81-110">Property</span></span>     | <span data-ttu-id="95c81-111">Тип</span><span class="sxs-lookup"><span data-stu-id="95c81-111">Type</span></span>        | <span data-ttu-id="95c81-112">Описание</span><span class="sxs-lookup"><span data-stu-id="95c81-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="95c81-113">аддитионалпропертиес</span><span class="sxs-lookup"><span data-stu-id="95c81-113">additionalProperties</span></span>|<span data-ttu-id="95c81-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="95c81-114">String collection</span></span>| <span data-ttu-id="95c81-115">Дополнительные свойства утверждения.</span><span class="sxs-lookup"><span data-stu-id="95c81-115">Additional properties of the claim.</span></span> <span data-ttu-id="95c81-116">Если свойство существует в этой коллекции, оно изменяет поведение необязательного утверждения, указанного в свойстве Name.</span><span class="sxs-lookup"><span data-stu-id="95c81-116">If a property exists in this collection, it modifies the behavior of the optional claim specified in the name property.</span></span> |
|<span data-ttu-id="95c81-117">основы</span><span class="sxs-lookup"><span data-stu-id="95c81-117">essential</span></span>|<span data-ttu-id="95c81-118">Логический</span><span class="sxs-lookup"><span data-stu-id="95c81-118">Boolean</span></span>| <span data-ttu-id="95c81-119">Если задано значение true, то требование, заданное клиентом, необходимо, чтобы обеспечить гладкую авторизацию для конкретной задачи, запрашиваемой конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="95c81-119">If the value is true, the claim specified by the client is necessary to ensure a smooth authorization experience for the specific task requested by the end user.</span></span> <span data-ttu-id="95c81-120">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="95c81-120">The default value is false.</span></span>|
|<span data-ttu-id="95c81-121">name</span><span class="sxs-lookup"><span data-stu-id="95c81-121">name</span></span>|<span data-ttu-id="95c81-122">String</span><span class="sxs-lookup"><span data-stu-id="95c81-122">String</span></span>| <span data-ttu-id="95c81-123">Имя необязательного утверждения.</span><span class="sxs-lookup"><span data-stu-id="95c81-123">The name of the optional claim.</span></span> |
|<span data-ttu-id="95c81-124">source</span><span class="sxs-lookup"><span data-stu-id="95c81-124">source</span></span>|<span data-ttu-id="95c81-125">String</span><span class="sxs-lookup"><span data-stu-id="95c81-125">String</span></span>| <span data-ttu-id="95c81-126">Источник утверждения (объект каталога).</span><span class="sxs-lookup"><span data-stu-id="95c81-126">The source (directory object) of the claim.</span></span> <span data-ttu-id="95c81-127">В свойствах расширения существуют предопределенные утверждения и пользовательские утверждения.</span><span class="sxs-lookup"><span data-stu-id="95c81-127">There are predefined claims and user-defined claims from extension properties.</span></span> <span data-ttu-id="95c81-128">Если исходное значение равно null, утверждение является предварительно определенным необязательным утверждением.</span><span class="sxs-lookup"><span data-stu-id="95c81-128">If the source value is null, the claim is a predefined optional claim.</span></span> <span data-ttu-id="95c81-129">Если исходное значение — User, то значение свойства Name — это свойство Extension объекта User.</span><span class="sxs-lookup"><span data-stu-id="95c81-129">If the source value is user, the value in the name property is the extension property from the user object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="95c81-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95c81-130">JSON representation</span></span>

<span data-ttu-id="95c81-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95c81-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.optionalClaim",
  "baseType": null
}-->

```json
{
  "additionalProperties": ["String"],
  "essential": true,
  "name": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "optionalClaim resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->