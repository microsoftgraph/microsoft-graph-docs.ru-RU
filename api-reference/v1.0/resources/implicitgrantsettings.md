---
title: Тип ресурса ИмплиЦитгрантсеттингс
description: Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0. Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса. Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 52c2929d36ceaa250bd3843556073190da9d4152
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939490"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="01198-105">Тип ресурса ИмплиЦитгрантсеттингс</span><span class="sxs-lookup"><span data-stu-id="01198-105">implicitGrantSettings resource type</span></span>

<span data-ttu-id="01198-106">Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="01198-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="01198-107">Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса.</span><span class="sxs-lookup"><span data-stu-id="01198-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="01198-108">Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.</span><span class="sxs-lookup"><span data-stu-id="01198-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="01198-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="01198-109">Properties</span></span>

| <span data-ttu-id="01198-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="01198-110">Property</span></span> | <span data-ttu-id="01198-111">Тип</span><span class="sxs-lookup"><span data-stu-id="01198-111">Type</span></span> | <span data-ttu-id="01198-112">Описание</span><span class="sxs-lookup"><span data-stu-id="01198-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="01198-113">енаблеидтокениссуанце</span><span class="sxs-lookup"><span data-stu-id="01198-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="01198-114">Логический</span><span class="sxs-lookup"><span data-stu-id="01198-114">Boolean</span></span> | <span data-ttu-id="01198-115">Указывает, может ли это веб-приложение запрашивать маркер идентификатора с помощью неявного потока OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="01198-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="01198-116">енаблеакцесстокениссуанце</span><span class="sxs-lookup"><span data-stu-id="01198-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="01198-117">Логический</span><span class="sxs-lookup"><span data-stu-id="01198-117">Boolean</span></span> | <span data-ttu-id="01198-118">Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="01198-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01198-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01198-119">JSON representation</span></span>
<span data-ttu-id="01198-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01198-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
