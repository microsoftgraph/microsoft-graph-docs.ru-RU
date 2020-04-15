---
title: Тип ресурса ИмплиЦитгрантсеттингс
description: Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0. Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса. Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 247d565e8b6c43b2ddedcdfeb23e3cd1fd5e3ad2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397469"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="9427f-105">Тип ресурса ИмплиЦитгрантсеттингс</span><span class="sxs-lookup"><span data-stu-id="9427f-105">implicitGrantSettings resource type</span></span>

<span data-ttu-id="9427f-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9427f-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9427f-107">Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="9427f-107">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="9427f-108">Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса.</span><span class="sxs-lookup"><span data-stu-id="9427f-108">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="9427f-109">Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.</span><span class="sxs-lookup"><span data-stu-id="9427f-109">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="9427f-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="9427f-110">Properties</span></span>

| <span data-ttu-id="9427f-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="9427f-111">Property</span></span> | <span data-ttu-id="9427f-112">Тип</span><span class="sxs-lookup"><span data-stu-id="9427f-112">Type</span></span> | <span data-ttu-id="9427f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9427f-113">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="9427f-114">енаблеидтокениссуанце</span><span class="sxs-lookup"><span data-stu-id="9427f-114">enableIdTokenIssuance</span></span>| <span data-ttu-id="9427f-115">Логический</span><span class="sxs-lookup"><span data-stu-id="9427f-115">Boolean</span></span> | <span data-ttu-id="9427f-116">Указывает, может ли это веб-приложение запрашивать маркер идентификатора с помощью неявного потока OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="9427f-116">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="9427f-117">енаблеакцесстокениссуанце</span><span class="sxs-lookup"><span data-stu-id="9427f-117">enableAccessTokenIssuance</span></span>| <span data-ttu-id="9427f-118">Логический</span><span class="sxs-lookup"><span data-stu-id="9427f-118">Boolean</span></span> | <span data-ttu-id="9427f-119">Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="9427f-119">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9427f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9427f-120">JSON representation</span></span>
<span data-ttu-id="9427f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9427f-121">Here is a JSON representation of the resource.</span></span>
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
