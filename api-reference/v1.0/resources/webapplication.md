---
title: Тип ресурса "приложение"
description: Указывает параметры для веб-приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c9b0c2f36913d3d89edb1bd119b2473158f0a9bb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939055"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="8fed2-103">Тип ресурса "приложение"</span><span class="sxs-lookup"><span data-stu-id="8fed2-103">webApplication resource type</span></span>

<span data-ttu-id="8fed2-104">Указывает параметры для веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="8fed2-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="8fed2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fed2-105">Properties</span></span>

| <span data-ttu-id="8fed2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fed2-106">Property</span></span> | <span data-ttu-id="8fed2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8fed2-107">Type</span></span> | <span data-ttu-id="8fed2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8fed2-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="8fed2-109">хомепажеурл</span><span class="sxs-lookup"><span data-stu-id="8fed2-109">homePageUrl</span></span> | <span data-ttu-id="8fed2-110">String</span><span class="sxs-lookup"><span data-stu-id="8fed2-110">String</span></span> | <span data-ttu-id="8fed2-111">Домашняя или целевая страница приложения.</span><span class="sxs-lookup"><span data-stu-id="8fed2-111">Home page or landing page of the application.</span></span> |
| <span data-ttu-id="8fed2-112">имплиЦитгрантсеттингс</span><span class="sxs-lookup"><span data-stu-id="8fed2-112">implicitGrantSettings</span></span> | [<span data-ttu-id="8fed2-113">имплиЦитгрантсеттингс</span><span class="sxs-lookup"><span data-stu-id="8fed2-113">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="8fed2-114">Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="8fed2-114">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| <span data-ttu-id="8fed2-115">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="8fed2-115">logoutUrl</span></span> | <span data-ttu-id="8fed2-116">String</span><span class="sxs-lookup"><span data-stu-id="8fed2-116">String</span></span> | <span data-ttu-id="8fed2-117">Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="8fed2-117">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| <span data-ttu-id="8fed2-118">редиректурис</span><span class="sxs-lookup"><span data-stu-id="8fed2-118">redirectUris</span></span> | <span data-ttu-id="8fed2-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8fed2-119">String collection</span></span> | <span data-ttu-id="8fed2-120">Задает URL-адреса, по которым маркеры пользователей отправляются для входа, или URI перенаправления, для которых отправляются коды авторизации OAuth 2,0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="8fed2-120">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8fed2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fed2-121">JSON representation</span></span>
<span data-ttu-id="8fed2-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fed2-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webApplication"
}-->

```json
{
  "homePageUrl": "String",
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
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
