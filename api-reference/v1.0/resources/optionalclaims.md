---
title: Тип Оптионалклаимс
description: Объявляет необязательные утверждения, запрошенные приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 19f5233ddb4db55f625460a063a175fc4a3e5efc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447278"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="ccaae-103">Тип ресурса Оптионалклаимс</span><span class="sxs-lookup"><span data-stu-id="ccaae-103">optionalClaims resource type</span></span>

<span data-ttu-id="ccaae-104">Пространство имен: Microsoft. Graph объявляет необязательные утверждения, запрошенные приложением.</span><span class="sxs-lookup"><span data-stu-id="ccaae-104">Namespace: microsoft.graph Declares the optional claims requested by an application.</span></span> <span data-ttu-id="ccaae-105">Приложение может настраивать дополнительные утверждения, возвращаемые в каждом из трех типов маркеров (маркер идентификатора, маркер доступа, маркер SAML 2), которые могут быть получены из службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="ccaae-105">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="ccaae-106">Приложение может настроить другой набор необязательных утверждений, которые будут возвращаться в каждом типе токена.</span><span class="sxs-lookup"><span data-stu-id="ccaae-106">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="ccaae-107">Свойство Оптионалклаимс [приложения](application.md) является объектом **оптионалклаимс** .</span><span class="sxs-lookup"><span data-stu-id="ccaae-107">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="ccaae-108">Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения им нужны в маркерах, отправляемых в приложения службой маркеров безопасности (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="ccaae-108">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="ccaae-109">Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="ccaae-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="ccaae-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="ccaae-110">Properties</span></span>
| <span data-ttu-id="ccaae-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccaae-111">Property</span></span>     | <span data-ttu-id="ccaae-112">Тип</span><span class="sxs-lookup"><span data-stu-id="ccaae-112">Type</span></span>        | <span data-ttu-id="ccaae-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ccaae-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ccaae-114">идтокен</span><span class="sxs-lookup"><span data-stu-id="ccaae-114">idToken</span></span>|<span data-ttu-id="ccaae-115">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="ccaae-115">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="ccaae-116">Необязательные утверждения, возвращенные в маркере идентификатора JWT.</span><span class="sxs-lookup"><span data-stu-id="ccaae-116">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="ccaae-117">accessToken</span><span class="sxs-lookup"><span data-stu-id="ccaae-117">accessToken</span></span>|<span data-ttu-id="ccaae-118">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="ccaae-118">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="ccaae-119">Необязательные утверждения, возвращенные в маркере доступа JWT.</span><span class="sxs-lookup"><span data-stu-id="ccaae-119">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="ccaae-120">saml2Token</span><span class="sxs-lookup"><span data-stu-id="ccaae-120">saml2Token</span></span>|<span data-ttu-id="ccaae-121">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="ccaae-121">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="ccaae-122">Необязательные утверждения, возвращенные в маркере SAML.</span><span class="sxs-lookup"><span data-stu-id="ccaae-122">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ccaae-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ccaae-123">JSON Representation</span></span>
<span data-ttu-id="ccaae-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccaae-124">Here is a JSON representation of the resource.</span></span>
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