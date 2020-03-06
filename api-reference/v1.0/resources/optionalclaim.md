---
title: Тип ресурса Оптионалклаим
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: sureshja
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: de97333a2a7580e9b6a9b58e042c0c5a8ff9bbe7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534131"
---
# <a name="optionalclaim-resource-type"></a><span data-ttu-id="f7462-103">Тип ресурса Оптионалклаим</span><span class="sxs-lookup"><span data-stu-id="f7462-103">optionalClaim resource type</span></span>

<span data-ttu-id="f7462-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7462-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7462-105">Содержит необязательное утверждение, связанное с [приложением](application.md)</span><span class="sxs-lookup"><span data-stu-id="f7462-105">Contains an optional claim associated with an [application](application.md)</span></span> <!-- or a service principal --><span data-ttu-id="f7462-106">.</span><span class="sxs-lookup"><span data-stu-id="f7462-106">.</span></span> <span data-ttu-id="f7462-107">Свойства `idToken`, `accessToken`и `saml2Token` , в ресурсе [оптионалклаимс](optionalclaims.md) , представляют собой коллекцию **оптионалклаим**.</span><span class="sxs-lookup"><span data-stu-id="f7462-107">The `idToken`, `accessToken`, and `saml2Token` properties of the [optionalClaims](optionalclaims.md) resource is a collection of **optionalClaim**.</span></span> <span data-ttu-id="f7462-108">Если это поддерживается определенным утверждением, вы также можете изменить поведение Оптионалклаим с помощью `additionalProperties` свойства.</span><span class="sxs-lookup"><span data-stu-id="f7462-108">If supported by a specific claim, you can also modify the behavior of the optionalClaim using the `additionalProperties` property.</span></span>

<span data-ttu-id="f7462-109">Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="f7462-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="f7462-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7462-110">Properties</span></span>

| <span data-ttu-id="f7462-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7462-111">Property</span></span>     | <span data-ttu-id="f7462-112">Тип</span><span class="sxs-lookup"><span data-stu-id="f7462-112">Type</span></span>        | <span data-ttu-id="f7462-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f7462-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7462-114">аддитионалпропертиес</span><span class="sxs-lookup"><span data-stu-id="f7462-114">additionalProperties</span></span>|<span data-ttu-id="f7462-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f7462-115">String collection</span></span>| <span data-ttu-id="f7462-116">Дополнительные свойства утверждения.</span><span class="sxs-lookup"><span data-stu-id="f7462-116">Additional properties of the claim.</span></span> <span data-ttu-id="f7462-117">Если свойство существует в этой коллекции, оно изменяет поведение необязательного утверждения, указанного в свойстве Name.</span><span class="sxs-lookup"><span data-stu-id="f7462-117">If a property exists in this collection, it modifies the behavior of the optional claim specified in the name property.</span></span> |
|<span data-ttu-id="f7462-118">основы</span><span class="sxs-lookup"><span data-stu-id="f7462-118">essential</span></span>|<span data-ttu-id="f7462-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7462-119">Boolean</span></span>| <span data-ttu-id="f7462-120">Если задано значение true, то требование, заданное клиентом, необходимо, чтобы обеспечить гладкую авторизацию для конкретной задачи, запрашиваемой конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="f7462-120">If the value is true, the claim specified by the client is necessary to ensure a smooth authorization experience for the specific task requested by the end user.</span></span> <span data-ttu-id="f7462-121">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="f7462-121">The default value is false.</span></span>|
|<span data-ttu-id="f7462-122">name</span><span class="sxs-lookup"><span data-stu-id="f7462-122">name</span></span>|<span data-ttu-id="f7462-123">String</span><span class="sxs-lookup"><span data-stu-id="f7462-123">String</span></span>| <span data-ttu-id="f7462-124">Имя необязательного утверждения.</span><span class="sxs-lookup"><span data-stu-id="f7462-124">The name of the optional claim.</span></span> |
|<span data-ttu-id="f7462-125">source</span><span class="sxs-lookup"><span data-stu-id="f7462-125">source</span></span>|<span data-ttu-id="f7462-126">Строка</span><span class="sxs-lookup"><span data-stu-id="f7462-126">String</span></span>| <span data-ttu-id="f7462-127">Источник утверждения (объект каталога).</span><span class="sxs-lookup"><span data-stu-id="f7462-127">The source (directory object) of the claim.</span></span> <span data-ttu-id="f7462-128">В свойствах расширения существуют предопределенные утверждения и пользовательские утверждения.</span><span class="sxs-lookup"><span data-stu-id="f7462-128">There are predefined claims and user-defined claims from extension properties.</span></span> <span data-ttu-id="f7462-129">Если исходное значение равно null, утверждение является предварительно определенным необязательным утверждением.</span><span class="sxs-lookup"><span data-stu-id="f7462-129">If the source value is null, the claim is a predefined optional claim.</span></span> <span data-ttu-id="f7462-130">Если исходное значение — User, то значение свойства Name — это свойство Extension объекта User.</span><span class="sxs-lookup"><span data-stu-id="f7462-130">If the source value is user, the value in the name property is the extension property from the user object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f7462-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7462-131">JSON representation</span></span>

<span data-ttu-id="f7462-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7462-132">The following is a JSON representation of the resource.</span></span>

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