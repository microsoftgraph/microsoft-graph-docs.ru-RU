---
title: тип веб-ресурса
description: Задает параметры для веб-приложения.
localization_priority: Normal
ms.openlocfilehash: 7e03977481f0c021b7d67ec44fd4db275642cdf8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527670"
---
# <a name="web-resource-type"></a><span data-ttu-id="5549f-103">тип веб-ресурса</span><span class="sxs-lookup"><span data-stu-id="5549f-103">web resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5549f-104">Задает параметры для веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="5549f-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="5549f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5549f-105">Properties</span></span>

| <span data-ttu-id="5549f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5549f-106">Property</span></span> | <span data-ttu-id="5549f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5549f-107">Type</span></span> | <span data-ttu-id="5549f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5549f-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="5549f-109">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="5549f-109">implicitGrantSettings</span></span>|[<span data-ttu-id="5549f-110">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="5549f-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="5549f-111">Разрешение запроса маркеры, с помощью поток неявных OAuth 2.0 этого веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="5549f-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="5549f-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="5549f-112">logoutUrl</span></span>|<span data-ttu-id="5549f-113">String</span><span class="sxs-lookup"><span data-stu-id="5549f-113">String</span></span>| <span data-ttu-id="5549f-114">Задает URL-адрес, который будет использоваться службой авторизации корпорации Майкрософт для выхода из системы на пользователя, с помощью [канала передний план](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [снова канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколы выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="5549f-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="5549f-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="5549f-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="5549f-116">Логическое</span><span class="sxs-lookup"><span data-stu-id="5549f-116">Boolean</span></span>| <span data-ttu-id="5549f-117">Нерекомендуемое</span><span class="sxs-lookup"><span data-stu-id="5549f-117">Deprecated.</span></span> <span data-ttu-id="5549f-118">Не используйте.</span><span class="sxs-lookup"><span data-stu-id="5549f-118">Do not use.</span></span> | 
|<span data-ttu-id="5549f-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="5549f-119">redirectUris</span></span>|<span data-ttu-id="5549f-120">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5549f-120">String collection</span></span>| <span data-ttu-id="5549f-121">Указывает URL-адресов, которые будут отправлены маркеры пользователя для входа в или отправки коды авторизации коды URI, OAuth 2.0 и маркеры доступа для перенаправления.</span><span class="sxs-lookup"><span data-stu-id="5549f-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5549f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5549f-122">JSON representation</span></span>
<span data-ttu-id="5549f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5549f-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.web"
}-->

```json
{
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
  "oauth2AllowImplicitFlow": false,
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/web.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
