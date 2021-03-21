---
title: Тип ресурса webApplication
description: Указывает параметры для веб-приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 68266c75995fed51038319cf50e0925d5057fa91
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964536"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="e3369-103">Тип ресурса webApplication</span><span class="sxs-lookup"><span data-stu-id="e3369-103">webApplication resource type</span></span>

<span data-ttu-id="e3369-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3369-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3369-105">Указывает параметры для веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="e3369-105">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="e3369-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3369-106">Properties</span></span>

| <span data-ttu-id="e3369-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3369-107">Property</span></span> | <span data-ttu-id="e3369-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e3369-108">Type</span></span> | <span data-ttu-id="e3369-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e3369-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="e3369-110">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="e3369-110">homePageUrl</span></span> | <span data-ttu-id="e3369-111">String</span><span class="sxs-lookup"><span data-stu-id="e3369-111">String</span></span> | <span data-ttu-id="e3369-112">Главная или начальная страница приложения.</span><span class="sxs-lookup"><span data-stu-id="e3369-112">Home page or landing page of the application.</span></span> |
| <span data-ttu-id="e3369-113">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="e3369-113">implicitGrantSettings</span></span> | [<span data-ttu-id="e3369-114">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="e3369-114">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="e3369-115">Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="e3369-115">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| <span data-ttu-id="e3369-116">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="e3369-116">logoutUrl</span></span> | <span data-ttu-id="e3369-117">String</span><span class="sxs-lookup"><span data-stu-id="e3369-117">String</span></span> | <span data-ttu-id="e3369-118">Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.</span><span class="sxs-lookup"><span data-stu-id="e3369-118">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| <span data-ttu-id="e3369-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="e3369-119">redirectUris</span></span> | <span data-ttu-id="e3369-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e3369-120">String collection</span></span> | <span data-ttu-id="e3369-121">Указывает URL-адреса, куда отправляются маркеры пользователей для регистрации, или URL-адреса перенаправления, куда отправляются коды авторизации OAuth 2.0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="e3369-121">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e3369-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3369-122">JSON representation</span></span>
<span data-ttu-id="e3369-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3369-123">Here is a JSON representation of the resource.</span></span>

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


