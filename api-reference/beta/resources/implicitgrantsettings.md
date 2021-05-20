---
title: неявный тип ресурсовGrantSettings
description: 'Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: fe471eefe817e48468258195dae4c93331dd6e04
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547017"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="302e3-103">неявный тип ресурсовGrantSettings</span><span class="sxs-lookup"><span data-stu-id="302e3-103">implicitGrantSettings resource type</span></span>

<span data-ttu-id="302e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="302e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="302e3-105">Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="302e3-105">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="302e3-106">Отдельные свойства доступны для запроса ID и маркеров доступа в рамках неявного потока.</span><span class="sxs-lookup"><span data-stu-id="302e3-106">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="302e3-107">Чтобы включить неявный поток, необходимо установить по крайней мере одно из следующих свойств.</span><span class="sxs-lookup"><span data-stu-id="302e3-107">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="302e3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="302e3-108">Properties</span></span>

| <span data-ttu-id="302e3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="302e3-109">Property</span></span> | <span data-ttu-id="302e3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="302e3-110">Type</span></span> | <span data-ttu-id="302e3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="302e3-111">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="302e3-112">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="302e3-112">enableIdTokenIssuance</span></span>| <span data-ttu-id="302e3-113">Логический</span><span class="sxs-lookup"><span data-stu-id="302e3-113">Boolean</span></span> | <span data-ttu-id="302e3-114">Указывает, может ли это веб-приложение запрашивать маркер ID с помощью неявного потока OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="302e3-114">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="302e3-115">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="302e3-115">enableAccessTokenIssuance</span></span>| <span data-ttu-id="302e3-116">Логический</span><span class="sxs-lookup"><span data-stu-id="302e3-116">Boolean</span></span> | <span data-ttu-id="302e3-117">Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="302e3-117">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="302e3-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="302e3-118">JSON representation</span></span>
<span data-ttu-id="302e3-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="302e3-119">Here is a JSON representation of the resource.</span></span>
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


