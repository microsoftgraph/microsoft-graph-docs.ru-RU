---
title: Тип ресурса ИмплиЦитгрантсеттингс
description: Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0. Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса. Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 86acc0228b14752d17e7c4c3d98c8ff9ea77503f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086657"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="92142-105">Тип ресурса ИмплиЦитгрантсеттингс</span><span class="sxs-lookup"><span data-stu-id="92142-105">implicitGrantSettings resource type</span></span>

<span data-ttu-id="92142-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92142-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92142-107">Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="92142-107">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="92142-108">Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса.</span><span class="sxs-lookup"><span data-stu-id="92142-108">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="92142-109">Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.</span><span class="sxs-lookup"><span data-stu-id="92142-109">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="92142-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="92142-110">Properties</span></span>

| <span data-ttu-id="92142-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="92142-111">Property</span></span> | <span data-ttu-id="92142-112">Тип</span><span class="sxs-lookup"><span data-stu-id="92142-112">Type</span></span> | <span data-ttu-id="92142-113">Описание</span><span class="sxs-lookup"><span data-stu-id="92142-113">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="92142-114">енаблеидтокениссуанце</span><span class="sxs-lookup"><span data-stu-id="92142-114">enableIdTokenIssuance</span></span>| <span data-ttu-id="92142-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="92142-115">Boolean</span></span> | <span data-ttu-id="92142-116">Указывает, может ли это веб-приложение запрашивать маркер идентификатора с помощью неявного потока OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="92142-116">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="92142-117">енаблеакцесстокениссуанце</span><span class="sxs-lookup"><span data-stu-id="92142-117">enableAccessTokenIssuance</span></span>| <span data-ttu-id="92142-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="92142-118">Boolean</span></span> | <span data-ttu-id="92142-119">Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="92142-119">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92142-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92142-120">JSON representation</span></span>
<span data-ttu-id="92142-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92142-121">Here is a JSON representation of the resource.</span></span>
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

