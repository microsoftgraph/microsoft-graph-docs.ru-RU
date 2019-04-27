---
title: Тип ресурса "приложение"
description: Указывает параметры для веб-приложения.
localization_priority: Normal
ms.openlocfilehash: cdb210d5193167138ecec216b1e4084554f05c78
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348433"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="8c0a5-103">Тип ресурса "приложение"</span><span class="sxs-lookup"><span data-stu-id="8c0a5-103">webApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c0a5-104">Указывает параметры для веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="8c0a5-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="8c0a5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c0a5-105">Properties</span></span>

| <span data-ttu-id="8c0a5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c0a5-106">Property</span></span> | <span data-ttu-id="8c0a5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8c0a5-107">Type</span></span> | <span data-ttu-id="8c0a5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8c0a5-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="8c0a5-109">ИмплиЦитгрантсеттингс</span><span class="sxs-lookup"><span data-stu-id="8c0a5-109">implicitGrantSettings</span></span>|[<span data-ttu-id="8c0a5-110">ИмплиЦитгрантсеттингс</span><span class="sxs-lookup"><span data-stu-id="8c0a5-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="8c0a5-111">Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="8c0a5-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="8c0a5-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="8c0a5-112">logoutUrl</span></span>|<span data-ttu-id="8c0a5-113">String</span><span class="sxs-lookup"><span data-stu-id="8c0a5-113">String</span></span>| <span data-ttu-id="8c0a5-114">Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="8c0a5-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="8c0a5-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="8c0a5-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="8c0a5-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c0a5-116">Boolean</span></span>| <span data-ttu-id="8c0a5-117">Устаревшие.</span><span class="sxs-lookup"><span data-stu-id="8c0a5-117">Deprecated.</span></span> <span data-ttu-id="8c0a5-118">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="8c0a5-118">Do not use.</span></span> | 
|<span data-ttu-id="8c0a5-119">Редиректурис</span><span class="sxs-lookup"><span data-stu-id="8c0a5-119">redirectUris</span></span>|<span data-ttu-id="8c0a5-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8c0a5-120">String collection</span></span>| <span data-ttu-id="8c0a5-121">Задает URL-адреса, на которые отправляются маркеры пользователей для входа, или URI перенаправления, на которые отправляются коды авторизации OAuth 2,0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="8c0a5-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8c0a5-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c0a5-122">JSON representation</span></span>
<span data-ttu-id="8c0a5-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c0a5-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webApplication"
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
  "description": "webApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
