---
title: Тип Оптионалклаимс
description: Объявляет необязательные утверждения, запрошенные приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: d6a07685760025cd4aa35429d657a6658dba92b4
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401124"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="e0c47-103">Тип ресурса Оптионалклаимс</span><span class="sxs-lookup"><span data-stu-id="e0c47-103">optionalClaims resource type</span></span>

<span data-ttu-id="e0c47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0c47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0c47-105">Объявляет необязательные утверждения, запрошенные приложением.</span><span class="sxs-lookup"><span data-stu-id="e0c47-105">Declares the optional claims requested by an application.</span></span> <span data-ttu-id="e0c47-106">Приложение может настраивать дополнительные утверждения, возвращаемые в каждом из трех типов маркеров (маркер идентификатора, маркер доступа, маркер SAML 2), которые могут быть получены из службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="e0c47-106">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="e0c47-107">Приложение может настроить другой набор необязательных утверждений, которые будут возвращаться в каждом типе токена.</span><span class="sxs-lookup"><span data-stu-id="e0c47-107">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="e0c47-108">Свойство Оптионалклаимс [приложения](application.md) является объектом **оптионалклаимс** .</span><span class="sxs-lookup"><span data-stu-id="e0c47-108">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="e0c47-109">Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения им нужны в маркерах, отправляемых в приложения службой маркеров безопасности (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="e0c47-109">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="e0c47-110">Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="e0c47-110">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="e0c47-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0c47-111">Properties</span></span>
| <span data-ttu-id="e0c47-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0c47-112">Property</span></span>     | <span data-ttu-id="e0c47-113">Тип</span><span class="sxs-lookup"><span data-stu-id="e0c47-113">Type</span></span>        | <span data-ttu-id="e0c47-114">Описание</span><span class="sxs-lookup"><span data-stu-id="e0c47-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0c47-115">идтокен</span><span class="sxs-lookup"><span data-stu-id="e0c47-115">idToken</span></span>|<span data-ttu-id="e0c47-116">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="e0c47-116">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="e0c47-117">Необязательные утверждения, возвращенные в маркере идентификатора JWT.</span><span class="sxs-lookup"><span data-stu-id="e0c47-117">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="e0c47-118">accessToken</span><span class="sxs-lookup"><span data-stu-id="e0c47-118">accessToken</span></span>|<span data-ttu-id="e0c47-119">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="e0c47-119">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="e0c47-120">Необязательные утверждения, возвращенные в маркере доступа JWT.</span><span class="sxs-lookup"><span data-stu-id="e0c47-120">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="e0c47-121">saml2Token</span><span class="sxs-lookup"><span data-stu-id="e0c47-121">saml2Token</span></span>|<span data-ttu-id="e0c47-122">Коллекция [оптионалклаим](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="e0c47-122">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="e0c47-123">Необязательные утверждения, возвращенные в маркере SAML.</span><span class="sxs-lookup"><span data-stu-id="e0c47-123">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0c47-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0c47-124">JSON Representation</span></span>
<span data-ttu-id="e0c47-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0c47-125">Here is a JSON representation of the resource.</span></span>
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