---
title: Тип ресурса optionalClaim
description: Содержит необязательное утверждение, связанное с приложением.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 5e21ab86fb3ef34edea546546211782906e04251
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128542"
---
# <a name="optionalclaim-resource-type"></a><span data-ttu-id="56c05-103">Тип ресурса optionalClaim</span><span class="sxs-lookup"><span data-stu-id="56c05-103">optionalClaim resource type</span></span>

<span data-ttu-id="56c05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56c05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56c05-105">Содержит необязательное утверждение, связанное с [приложением](application.md)</span><span class="sxs-lookup"><span data-stu-id="56c05-105">Contains an optional claim associated with an [application](application.md)</span></span> <!-- or a service principal --><span data-ttu-id="56c05-106">.</span><span class="sxs-lookup"><span data-stu-id="56c05-106">.</span></span> <span data-ttu-id="56c05-107">Свойства **idToken,** **accessToken** и **saml2Token** ресурса [optionalClaims](optionalclaims.md) — это коллекция **optionalClaim.**</span><span class="sxs-lookup"><span data-stu-id="56c05-107">The **idToken**, **accessToken**, and **saml2Token** properties of the [optionalClaims](optionalclaims.md) resource is a collection of **optionalClaim**.</span></span> <span data-ttu-id="56c05-108">Если поддерживается определенным утверждением, можно также изменить поведение optionalClaim с помощью `additionalProperties` свойства.</span><span class="sxs-lookup"><span data-stu-id="56c05-108">If supported by a specific claim, you can also modify the behavior of the optionalClaim using the `additionalProperties` property.</span></span> 

<span data-ttu-id="56c05-109">Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="56c05-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="56c05-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="56c05-110">Properties</span></span>

| <span data-ttu-id="56c05-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="56c05-111">Property</span></span>     | <span data-ttu-id="56c05-112">Тип</span><span class="sxs-lookup"><span data-stu-id="56c05-112">Type</span></span>        | <span data-ttu-id="56c05-113">Описание</span><span class="sxs-lookup"><span data-stu-id="56c05-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="56c05-114">additionalProperties</span><span class="sxs-lookup"><span data-stu-id="56c05-114">additionalProperties</span></span>|<span data-ttu-id="56c05-115">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="56c05-115">String collection</span></span>| <span data-ttu-id="56c05-116">Дополнительные свойства утверждения.</span><span class="sxs-lookup"><span data-stu-id="56c05-116">Additional properties of the claim.</span></span> <span data-ttu-id="56c05-117">Если свойство существует в этой коллекции, оно изменяет поведение необязательного утверждения, указанного в свойстве name.</span><span class="sxs-lookup"><span data-stu-id="56c05-117">If a property exists in this collection, it modifies the behavior of the optional claim specified in the name property.</span></span> |
|<span data-ttu-id="56c05-118">essential</span><span class="sxs-lookup"><span data-stu-id="56c05-118">essential</span></span>|<span data-ttu-id="56c05-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="56c05-119">Boolean</span></span>| <span data-ttu-id="56c05-120">Если значение имеет значение true, утверждение, указанное клиентом, необходимо для обеспечения плавной авторизации для конкретной задачи, запрашиваемой конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="56c05-120">If the value is true, the claim specified by the client is necessary to ensure a smooth authorization experience for the specific task requested by the end user.</span></span> <span data-ttu-id="56c05-121">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="56c05-121">The default value is false.</span></span>|
|<span data-ttu-id="56c05-122">name</span><span class="sxs-lookup"><span data-stu-id="56c05-122">name</span></span>|<span data-ttu-id="56c05-123">String</span><span class="sxs-lookup"><span data-stu-id="56c05-123">String</span></span>| <span data-ttu-id="56c05-124">Имя необязательного утверждения.</span><span class="sxs-lookup"><span data-stu-id="56c05-124">The name of the optional claim.</span></span> |
|<span data-ttu-id="56c05-125">source</span><span class="sxs-lookup"><span data-stu-id="56c05-125">source</span></span>|<span data-ttu-id="56c05-126">Строка</span><span class="sxs-lookup"><span data-stu-id="56c05-126">String</span></span>| <span data-ttu-id="56c05-127">Источник (объект каталога) утверждения.</span><span class="sxs-lookup"><span data-stu-id="56c05-127">The source (directory object) of the claim.</span></span> <span data-ttu-id="56c05-128">Существуют предварительно определенные утверждения и пользовательские утверждения из свойств расширения.</span><span class="sxs-lookup"><span data-stu-id="56c05-128">There are predefined claims and user-defined claims from extension properties.</span></span> <span data-ttu-id="56c05-129">Если значение источника — null, утверждение является предварительно заранее задаваемой необязательной заявкой.</span><span class="sxs-lookup"><span data-stu-id="56c05-129">If the source value is null, the claim is a predefined optional claim.</span></span> <span data-ttu-id="56c05-130">Если исходным значением является пользователь, значением в свойстве name является свойство расширения объекта user.</span><span class="sxs-lookup"><span data-stu-id="56c05-130">If the source value is user, the value in the name property is the extension property from the user object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="56c05-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="56c05-131">JSON representation</span></span>

<span data-ttu-id="56c05-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56c05-132">The following is a JSON representation of the resource.</span></span>

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
