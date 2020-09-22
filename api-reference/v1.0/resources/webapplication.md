---
title: Тип ресурса "приложение"
description: Указывает параметры для веб-приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: aae3184a025757b910e0b19daa8a8d8057128506
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015262"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="68542-103">Тип ресурса "приложение"</span><span class="sxs-lookup"><span data-stu-id="68542-103">webApplication resource type</span></span>

<span data-ttu-id="68542-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68542-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68542-105">Указывает параметры для веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="68542-105">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="68542-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="68542-106">Properties</span></span>

| <span data-ttu-id="68542-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="68542-107">Property</span></span> | <span data-ttu-id="68542-108">Тип</span><span class="sxs-lookup"><span data-stu-id="68542-108">Type</span></span> | <span data-ttu-id="68542-109">Описание</span><span class="sxs-lookup"><span data-stu-id="68542-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="68542-110">хомепажеурл</span><span class="sxs-lookup"><span data-stu-id="68542-110">homePageUrl</span></span> | <span data-ttu-id="68542-111">String</span><span class="sxs-lookup"><span data-stu-id="68542-111">String</span></span> | <span data-ttu-id="68542-112">Главная или начальная страница приложения.</span><span class="sxs-lookup"><span data-stu-id="68542-112">Home page or landing page of the application.</span></span> |
| <span data-ttu-id="68542-113">имплиЦитгрантсеттингс</span><span class="sxs-lookup"><span data-stu-id="68542-113">implicitGrantSettings</span></span> | [<span data-ttu-id="68542-114">имплиЦитгрантсеттингс</span><span class="sxs-lookup"><span data-stu-id="68542-114">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="68542-115">Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="68542-115">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| <span data-ttu-id="68542-116">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="68542-116">logoutUrl</span></span> | <span data-ttu-id="68542-117">String</span><span class="sxs-lookup"><span data-stu-id="68542-117">String</span></span> | <span data-ttu-id="68542-118">Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="68542-118">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| <span data-ttu-id="68542-119">редиректурис</span><span class="sxs-lookup"><span data-stu-id="68542-119">redirectUris</span></span> | <span data-ttu-id="68542-120">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="68542-120">String collection</span></span> | <span data-ttu-id="68542-121">Задает URL-адреса, по которым маркеры пользователей отправляются для входа, или URI перенаправления, для которых отправляются коды авторизации OAuth 2,0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="68542-121">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="68542-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68542-122">JSON representation</span></span>
<span data-ttu-id="68542-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68542-123">Here is a JSON representation of the resource.</span></span>

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

