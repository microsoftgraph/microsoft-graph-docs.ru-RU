---
title: Тип ресурса implicitGrantSettings
description: Разрешение запроса маркеры, с помощью поток неявных OAuth 2.0 этого веб-приложения. Отдельные свойства доступны для запроса маркеры идентификатор и доступа как часть неявных потока. Чтобы включить неявных поток, по крайней мере одного из следующих свойств необходимо установить значение true.
ms.openlocfilehash: 018cd422b56724811e1913ff0e94aea16d7c68f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077140"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="a9ac4-105">Тип ресурса implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="a9ac4-105">implicitGrantSettings resource type</span></span>

> <span data-ttu-id="a9ac4-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a9ac4-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9ac4-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9ac4-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9ac4-108">Разрешение запроса маркеры, с помощью поток неявных OAuth 2.0 этого веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="a9ac4-108">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="a9ac4-109">Отдельные свойства доступны для запроса маркеры идентификатор и доступа как часть неявных потока.</span><span class="sxs-lookup"><span data-stu-id="a9ac4-109">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="a9ac4-110">Чтобы включить неявных поток, по крайней мере одного из следующих свойств необходимо установить значение true.</span><span class="sxs-lookup"><span data-stu-id="a9ac4-110">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="a9ac4-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9ac4-111">Properties</span></span>

| <span data-ttu-id="a9ac4-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9ac4-112">Property</span></span> | <span data-ttu-id="a9ac4-113">Тип</span><span class="sxs-lookup"><span data-stu-id="a9ac4-113">Type</span></span> | <span data-ttu-id="a9ac4-114">Description</span><span class="sxs-lookup"><span data-stu-id="a9ac4-114">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="a9ac4-115">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="a9ac4-115">enableIdTokenIssuance</span></span>| <span data-ttu-id="a9ac4-116">Логический</span><span class="sxs-lookup"><span data-stu-id="a9ac4-116">Boolean</span></span> | <span data-ttu-id="a9ac4-117">Разрешение запроса с помощью поток неявных OAuth 2.0 маркера Идентификации данного веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="a9ac4-117">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="a9ac4-118">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="a9ac4-118">enableAccessTokenIssuance</span></span>| <span data-ttu-id="a9ac4-119">Логический</span><span class="sxs-lookup"><span data-stu-id="a9ac4-119">Boolean</span></span> | <span data-ttu-id="a9ac4-120">Разрешение запроса маркер доступа с помощью поток неявных OAuth 2.0 этого веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="a9ac4-120">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9ac4-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9ac4-121">JSON representation</span></span>
<span data-ttu-id="a9ac4-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9ac4-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
