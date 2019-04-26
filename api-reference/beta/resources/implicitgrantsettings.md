---
title: Тип ресурса ИмплиЦитгрантсеттингс
description: Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0. Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса. Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.
localization_priority: Normal
ms.openlocfilehash: 1026f3b97a3305dff7a715fae000ab9695ac8e9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333612"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="efca7-105">Тип ресурса ИмплиЦитгрантсеттингс</span><span class="sxs-lookup"><span data-stu-id="efca7-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efca7-106">Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="efca7-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="efca7-107">Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса.</span><span class="sxs-lookup"><span data-stu-id="efca7-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="efca7-108">Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.</span><span class="sxs-lookup"><span data-stu-id="efca7-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="efca7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="efca7-109">Properties</span></span>

| <span data-ttu-id="efca7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="efca7-110">Property</span></span> | <span data-ttu-id="efca7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="efca7-111">Type</span></span> | <span data-ttu-id="efca7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="efca7-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="efca7-113">Енаблеидтокениссуанце</span><span class="sxs-lookup"><span data-stu-id="efca7-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="efca7-114">Логический</span><span class="sxs-lookup"><span data-stu-id="efca7-114">Boolean</span></span> | <span data-ttu-id="efca7-115">Указывает, может ли это веб-приложение запрашивать маркер идентификатора с помощью неявного потока OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="efca7-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="efca7-116">Енаблеакцесстокениссуанце</span><span class="sxs-lookup"><span data-stu-id="efca7-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="efca7-117">Логический</span><span class="sxs-lookup"><span data-stu-id="efca7-117">Boolean</span></span> | <span data-ttu-id="efca7-118">Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="efca7-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efca7-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efca7-119">JSON representation</span></span>
<span data-ttu-id="efca7-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efca7-120">Here is a JSON representation of the resource.</span></span>
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
