---
title: Тип ресурса implicitGrantSettings
description: Разрешение запроса маркеры, с помощью поток неявных OAuth 2.0 этого веб-приложения. Отдельные свойства доступны для запроса маркеры идентификатор и доступа как часть неявных потока. Чтобы включить неявных поток, по крайней мере одного из следующих свойств необходимо установить значение true.
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520566"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="44234-105">Тип ресурса implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="44234-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44234-106">Разрешение запроса маркеры, с помощью поток неявных OAuth 2.0 этого веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="44234-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="44234-107">Отдельные свойства доступны для запроса маркеры идентификатор и доступа как часть неявных потока.</span><span class="sxs-lookup"><span data-stu-id="44234-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="44234-108">Чтобы включить неявных поток, по крайней мере одного из следующих свойств необходимо установить значение true.</span><span class="sxs-lookup"><span data-stu-id="44234-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="44234-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="44234-109">Properties</span></span>

| <span data-ttu-id="44234-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="44234-110">Property</span></span> | <span data-ttu-id="44234-111">Тип</span><span class="sxs-lookup"><span data-stu-id="44234-111">Type</span></span> | <span data-ttu-id="44234-112">Описание</span><span class="sxs-lookup"><span data-stu-id="44234-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="44234-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="44234-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="44234-114">Логическое</span><span class="sxs-lookup"><span data-stu-id="44234-114">Boolean</span></span> | <span data-ttu-id="44234-115">Разрешение запроса с помощью поток неявных OAuth 2.0 маркера Идентификации данного веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="44234-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="44234-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="44234-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="44234-117">Логическое</span><span class="sxs-lookup"><span data-stu-id="44234-117">Boolean</span></span> | <span data-ttu-id="44234-118">Разрешение запроса маркер доступа с помощью поток неявных OAuth 2.0 этого веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="44234-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44234-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44234-119">JSON representation</span></span>
<span data-ttu-id="44234-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44234-120">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/implicitgrantsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
