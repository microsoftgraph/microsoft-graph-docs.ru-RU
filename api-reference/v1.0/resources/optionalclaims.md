---
title: Тип optionalClaims
description: Объявляет необязательные утверждения, запрашиваемые приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 2830aef91557346d3d02249d35df41eccffa565e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136222"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="785ad-103">Тип ресурса optionalClaims</span><span class="sxs-lookup"><span data-stu-id="785ad-103">optionalClaims resource type</span></span>

<span data-ttu-id="785ad-104">Пространство имен: microsoft.graph объявляет необязательные утверждения, запрашиваемые приложением.</span><span class="sxs-lookup"><span data-stu-id="785ad-104">Namespace: microsoft.graph Declares the optional claims requested by an application.</span></span> <span data-ttu-id="785ad-105">Приложение может настроить необязательные утверждения, возвращаемые в каждом из трех типов маркеров (маркера ИД, маркера доступа, маркера SAML 2), которые оно может получить от службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="785ad-105">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="785ad-106">Приложение может настроить другой набор необязательных утверждений, возвращаемых в каждом типе маркера.</span><span class="sxs-lookup"><span data-stu-id="785ad-106">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="785ad-107">Свойство optionalClaims приложения [является](application.md) **объектом optionalClaims.**</span><span class="sxs-lookup"><span data-stu-id="785ad-107">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="785ad-108">Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения им нужны в маркерах, отправляемых в приложения службой маркеров безопасности (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="785ad-108">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="785ad-109">Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="785ad-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="785ad-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="785ad-110">Properties</span></span>
| <span data-ttu-id="785ad-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="785ad-111">Property</span></span>     | <span data-ttu-id="785ad-112">Тип</span><span class="sxs-lookup"><span data-stu-id="785ad-112">Type</span></span>        | <span data-ttu-id="785ad-113">Описание</span><span class="sxs-lookup"><span data-stu-id="785ad-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="785ad-114">idToken</span><span class="sxs-lookup"><span data-stu-id="785ad-114">idToken</span></span>|<span data-ttu-id="785ad-115">[Коллекция optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="785ad-115">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="785ad-116">Необязательные утверждения, возвращенные в маркере JWT ID.</span><span class="sxs-lookup"><span data-stu-id="785ad-116">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="785ad-117">accessToken</span><span class="sxs-lookup"><span data-stu-id="785ad-117">accessToken</span></span>|<span data-ttu-id="785ad-118">[Коллекция optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="785ad-118">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="785ad-119">Необязательные утверждения, возвращенные в маркере доступа JWT.</span><span class="sxs-lookup"><span data-stu-id="785ad-119">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="785ad-120">saml2Token</span><span class="sxs-lookup"><span data-stu-id="785ad-120">saml2Token</span></span>|<span data-ttu-id="785ad-121">[Коллекция optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="785ad-121">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="785ad-122">Необязательные утверждения, возвращенные в маркере SAML.</span><span class="sxs-lookup"><span data-stu-id="785ad-122">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="785ad-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="785ad-123">JSON Representation</span></span>
<span data-ttu-id="785ad-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="785ad-124">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.optionalClaims"
}-->
``` json
{
  "idToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "accessToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "saml2Token": [{"@odata.type": "microsoft.graph.optionalClaim"}]
}
```
