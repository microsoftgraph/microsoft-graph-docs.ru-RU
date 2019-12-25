---
title: Тип Оптионалклаимс
description: Объявляет необязательные утверждения, запрошенные приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 4c768c09b0755327ff6fbd7b2de0feb906944fbf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863836"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="e2e1f-103">Тип ресурса Оптионалклаимс</span><span class="sxs-lookup"><span data-stu-id="e2e1f-103">optionalClaims resource type</span></span>
<span data-ttu-id="e2e1f-104">Объявляет необязательные утверждения, запрошенные приложением.</span><span class="sxs-lookup"><span data-stu-id="e2e1f-104">Declares the optional claims requested by an application.</span></span> <span data-ttu-id="e2e1f-105">Приложение может настраивать дополнительные утверждения, возвращаемые в каждом из трех типов маркеров (маркер идентификатора, маркер доступа, маркер SAML 2), которые могут быть получены из службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="e2e1f-105">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="e2e1f-106">Приложение может настроить другой набор необязательных утверждений, которые будут возвращаться в каждом типе токена.</span><span class="sxs-lookup"><span data-stu-id="e2e1f-106">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="e2e1f-107">Свойство Оптионалклаимс [приложения](application.md) является объектом **оптионалклаимс** .</span><span class="sxs-lookup"><span data-stu-id="e2e1f-107">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="e2e1f-108">Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения им нужны в маркерах, отправляемых в приложения службой маркеров безопасности (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="e2e1f-108">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="e2e1f-109">Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="e2e1f-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="e2e1f-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2e1f-110">Properties</span></span>
| <span data-ttu-id="e2e1f-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2e1f-111">Property</span></span>     | <span data-ttu-id="e2e1f-112">Тип</span><span class="sxs-lookup"><span data-stu-id="e2e1f-112">Type</span></span>        | <span data-ttu-id="e2e1f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e2e1f-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2e1f-114">идтокен</span><span class="sxs-lookup"><span data-stu-id="e2e1f-114">idToken</span></span>|<span data-ttu-id="e2e1f-115">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="e2e1f-115">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="e2e1f-116">Необязательные утверждения, возвращенные в маркере идентификатора JWT.</span><span class="sxs-lookup"><span data-stu-id="e2e1f-116">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="e2e1f-117">accessToken</span><span class="sxs-lookup"><span data-stu-id="e2e1f-117">accessToken</span></span>|<span data-ttu-id="e2e1f-118">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="e2e1f-118">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="e2e1f-119">Необязательные утверждения, возвращенные в маркере доступа JWT.</span><span class="sxs-lookup"><span data-stu-id="e2e1f-119">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="e2e1f-120">saml2Token</span><span class="sxs-lookup"><span data-stu-id="e2e1f-120">saml2Token</span></span>|<span data-ttu-id="e2e1f-121">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="e2e1f-121">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="e2e1f-122">Необязательные утверждения, возвращенные в маркере SAML.</span><span class="sxs-lookup"><span data-stu-id="e2e1f-122">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2e1f-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2e1f-123">JSON Representation</span></span>
<span data-ttu-id="e2e1f-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2e1f-124">Here is a JSON representation of the resource.</span></span>
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