---
title: Тип Оптионалклаимс
description: Объявляет необязательные утверждения, запрошенные приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 40f8fd033f5fd5bda5605e7df66ee80b21acfe51
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43389003"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="f0892-103">Тип ресурса Оптионалклаимс</span><span class="sxs-lookup"><span data-stu-id="f0892-103">optionalClaims resource type</span></span>

<span data-ttu-id="f0892-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0892-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0892-105">Объявляет необязательные утверждения, запрошенные приложением.</span><span class="sxs-lookup"><span data-stu-id="f0892-105">Declares the optional claims requested by an application.</span></span> <span data-ttu-id="f0892-106">Приложение может настраивать дополнительные утверждения, возвращаемые в каждом из трех типов маркеров (маркер идентификатора, маркер доступа, маркер SAML 2), которые могут быть получены из службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="f0892-106">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="f0892-107">Приложение может настроить другой набор необязательных утверждений, которые будут возвращаться в каждом типе токена.</span><span class="sxs-lookup"><span data-stu-id="f0892-107">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="f0892-108">Свойство Оптионалклаимс [приложения](application.md) является объектом **оптионалклаимс** .</span><span class="sxs-lookup"><span data-stu-id="f0892-108">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="f0892-109">Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения им нужны в маркерах, отправляемых в приложения службой маркеров безопасности (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="f0892-109">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="f0892-110">Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="f0892-110">See [provide optional claims to your Azure AD app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="f0892-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0892-111">Properties</span></span>
| <span data-ttu-id="f0892-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0892-112">Property</span></span>     | <span data-ttu-id="f0892-113">Тип</span><span class="sxs-lookup"><span data-stu-id="f0892-113">Type</span></span>        | <span data-ttu-id="f0892-114">Описание</span><span class="sxs-lookup"><span data-stu-id="f0892-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f0892-115">идтокен</span><span class="sxs-lookup"><span data-stu-id="f0892-115">idToken</span></span>|<span data-ttu-id="f0892-116">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="f0892-116">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="f0892-117">Необязательные утверждения, возвращенные в маркере идентификатора JWT.</span><span class="sxs-lookup"><span data-stu-id="f0892-117">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="f0892-118">accessToken</span><span class="sxs-lookup"><span data-stu-id="f0892-118">accessToken</span></span>|<span data-ttu-id="f0892-119">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="f0892-119">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="f0892-120">Необязательные утверждения, возвращенные в маркере доступа JWT.</span><span class="sxs-lookup"><span data-stu-id="f0892-120">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="f0892-121">saml2Token</span><span class="sxs-lookup"><span data-stu-id="f0892-121">saml2Token</span></span>|<span data-ttu-id="f0892-122">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="f0892-122">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="f0892-123">Необязательные утверждения, возвращенные в маркере SAML.</span><span class="sxs-lookup"><span data-stu-id="f0892-123">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0892-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0892-124">JSON Representation</span></span>
<span data-ttu-id="f0892-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0892-125">Here is a JSON representation of the resource.</span></span>
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
