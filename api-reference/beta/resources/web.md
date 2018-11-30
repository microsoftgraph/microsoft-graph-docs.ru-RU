---
title: тип веб-ресурса
description: Задает параметры для веб-приложения.
ms.openlocfilehash: c040de0c323e57f20e04dcf662ea088b1018c144
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080737"
---
# <a name="web-resource-type"></a><span data-ttu-id="ac043-103">тип веб-ресурса</span><span class="sxs-lookup"><span data-stu-id="ac043-103">web resource type</span></span>

> <span data-ttu-id="ac043-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ac043-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac043-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac043-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac043-106">Задает параметры для веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="ac043-106">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="ac043-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac043-107">Properties</span></span>

| <span data-ttu-id="ac043-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac043-108">Property</span></span> | <span data-ttu-id="ac043-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ac043-109">Type</span></span> | <span data-ttu-id="ac043-110">Description</span><span class="sxs-lookup"><span data-stu-id="ac043-110">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="ac043-111">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="ac043-111">implicitGrantSettings</span></span>|[<span data-ttu-id="ac043-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="ac043-112">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="ac043-113">Разрешение запроса маркеры, с помощью поток неявных OAuth 2.0 этого веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="ac043-113">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="ac043-114">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="ac043-114">logoutUrl</span></span>|<span data-ttu-id="ac043-115">String</span><span class="sxs-lookup"><span data-stu-id="ac043-115">String</span></span>| <span data-ttu-id="ac043-116">Задает URL-адрес, который будет использоваться службой авторизации корпорации Майкрософт для выхода из системы на пользователя, с помощью [канала передний план](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [снова канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколы выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="ac043-116">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="ac043-117">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="ac043-117">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="ac043-118">Логический</span><span class="sxs-lookup"><span data-stu-id="ac043-118">Boolean</span></span>| <span data-ttu-id="ac043-119">Рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="ac043-119">Deprecated.</span></span> <span data-ttu-id="ac043-120">Не используйте.</span><span class="sxs-lookup"><span data-stu-id="ac043-120">Do not use.</span></span> | 
|<span data-ttu-id="ac043-121">redirectUris</span><span class="sxs-lookup"><span data-stu-id="ac043-121">redirectUris</span></span>|<span data-ttu-id="ac043-122">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ac043-122">String collection</span></span>| <span data-ttu-id="ac043-123">Указывает URL-адресов, которые будут отправлены маркеры пользователя для входа в или отправки коды авторизации коды URI, OAuth 2.0 и маркеры доступа для перенаправления.</span><span class="sxs-lookup"><span data-stu-id="ac043-123">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ac043-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac043-124">JSON representation</span></span>
<span data-ttu-id="ac043-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac043-125">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
