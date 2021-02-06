---
title: Тип ресурса webApplication
description: Указывает параметры для веб-приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 630423c787f8a89734c56362b079a402a5606929
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135620"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="783de-103">Тип ресурса webApplication</span><span class="sxs-lookup"><span data-stu-id="783de-103">webApplication resource type</span></span>

<span data-ttu-id="783de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="783de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="783de-105">Указывает параметры для веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="783de-105">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="783de-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="783de-106">Properties</span></span>

| <span data-ttu-id="783de-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="783de-107">Property</span></span> | <span data-ttu-id="783de-108">Тип</span><span class="sxs-lookup"><span data-stu-id="783de-108">Type</span></span> | <span data-ttu-id="783de-109">Описание</span><span class="sxs-lookup"><span data-stu-id="783de-109">Description</span></span> |
|:---------|:-----|:------------|
| `homePageUrl` | <span data-ttu-id="783de-110">String</span><span class="sxs-lookup"><span data-stu-id="783de-110">String</span></span> | <span data-ttu-id="783de-111">Главная или начальная страница приложения.</span><span class="sxs-lookup"><span data-stu-id="783de-111">Home page or landing page of the application.</span></span> |
| `implicitGrantSettings` | [<span data-ttu-id="783de-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="783de-112">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="783de-113">Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="783de-113">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| `logoutUrl` | <span data-ttu-id="783de-114">String</span><span class="sxs-lookup"><span data-stu-id="783de-114">String</span></span> | <span data-ttu-id="783de-115">Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="783de-115">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| `redirectUris` | <span data-ttu-id="783de-116">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="783de-116">String collection</span></span> | <span data-ttu-id="783de-117">Указывает URL-адреса, в которые отправляются маркеры пользователей для входов, или URIS перенаправления, в которые отправляются коды авторизации OAuth 2.0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="783de-117">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="783de-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="783de-118">JSON representation</span></span>
<span data-ttu-id="783de-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="783de-119">Here is a JSON representation of the resource.</span></span>

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


