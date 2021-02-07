---
title: Тип ресурса implicitGrantSettings
description: Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0. Отдельные свойства доступны для запроса ИД и маркеров доступа в рамках неявного потока. Чтобы включить неявный поток, по крайней мере одно из следующих свойств должно иметь true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 58509ff0f0264a683aaae9c83d60e0f041ef0af7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133282"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="0a5b8-105">Тип ресурса implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="0a5b8-105">implicitGrantSettings resource type</span></span>

<span data-ttu-id="0a5b8-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a5b8-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0a5b8-107">Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="0a5b8-107">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="0a5b8-108">Отдельные свойства доступны для запроса ИД и маркеров доступа в рамках неявного потока.</span><span class="sxs-lookup"><span data-stu-id="0a5b8-108">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="0a5b8-109">Чтобы включить неявный поток, по крайней мере одно из следующих свойств должно иметь true.</span><span class="sxs-lookup"><span data-stu-id="0a5b8-109">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="0a5b8-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a5b8-110">Properties</span></span>

| <span data-ttu-id="0a5b8-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a5b8-111">Property</span></span> | <span data-ttu-id="0a5b8-112">Тип</span><span class="sxs-lookup"><span data-stu-id="0a5b8-112">Type</span></span> | <span data-ttu-id="0a5b8-113">Описание</span><span class="sxs-lookup"><span data-stu-id="0a5b8-113">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="0a5b8-114">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="0a5b8-114">enableIdTokenIssuance</span></span>| <span data-ttu-id="0a5b8-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a5b8-115">Boolean</span></span> | <span data-ttu-id="0a5b8-116">Указывает, может ли это веб-приложение запрашивать маркер ИД с помощью неявного потока OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="0a5b8-116">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="0a5b8-117">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="0a5b8-117">enableAccessTokenIssuance</span></span>| <span data-ttu-id="0a5b8-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a5b8-118">Boolean</span></span> | <span data-ttu-id="0a5b8-119">Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="0a5b8-119">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a5b8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a5b8-120">JSON representation</span></span>
<span data-ttu-id="0a5b8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a5b8-121">Here is a JSON representation of the resource.</span></span>
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

