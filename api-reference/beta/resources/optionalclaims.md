---
title: Тип optionalClaims
description: Объявляет необязательные утверждения, запрашиваемые приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d50b514fa29cf99f22bb42238ac9d6a66126ab53
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132659"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="bf8f6-103">Тип ресурса optionalClaims</span><span class="sxs-lookup"><span data-stu-id="bf8f6-103">optionalClaims resource type</span></span>

<span data-ttu-id="bf8f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf8f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf8f6-105">Объявляет необязательные утверждения, запрашиваемые приложением.</span><span class="sxs-lookup"><span data-stu-id="bf8f6-105">Declares the optional claims requested by an application.</span></span> <span data-ttu-id="bf8f6-106">Приложение может настроить необязательные утверждения, возвращаемые в каждом из трех типов маркеров (маркера ИД, маркера доступа, маркера SAML 2), которые оно может получить от службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="bf8f6-106">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="bf8f6-107">Приложение может настроить другой набор необязательных утверждений, возвращаемых в каждом типе маркера.</span><span class="sxs-lookup"><span data-stu-id="bf8f6-107">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="bf8f6-108">Свойство optionalClaims приложения [является](application.md) **объектом optionalClaims.**</span><span class="sxs-lookup"><span data-stu-id="bf8f6-108">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="bf8f6-109">Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения им нужны в маркерах, отправляемых в приложения службой маркеров безопасности (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="bf8f6-109">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="bf8f6-110">Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="bf8f6-110">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="bf8f6-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf8f6-111">Properties</span></span>
| <span data-ttu-id="bf8f6-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf8f6-112">Property</span></span>     | <span data-ttu-id="bf8f6-113">Тип</span><span class="sxs-lookup"><span data-stu-id="bf8f6-113">Type</span></span>        | <span data-ttu-id="bf8f6-114">Описание</span><span class="sxs-lookup"><span data-stu-id="bf8f6-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bf8f6-115">idToken</span><span class="sxs-lookup"><span data-stu-id="bf8f6-115">idToken</span></span>|<span data-ttu-id="bf8f6-116">[Коллекция optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="bf8f6-116">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="bf8f6-117">Необязательные утверждения, возвращенные в маркере JWT ID.</span><span class="sxs-lookup"><span data-stu-id="bf8f6-117">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="bf8f6-118">accessToken</span><span class="sxs-lookup"><span data-stu-id="bf8f6-118">accessToken</span></span>|<span data-ttu-id="bf8f6-119">[Коллекция optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="bf8f6-119">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="bf8f6-120">Необязательные утверждения, возвращенные в маркере доступа JWT.</span><span class="sxs-lookup"><span data-stu-id="bf8f6-120">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="bf8f6-121">saml2Token</span><span class="sxs-lookup"><span data-stu-id="bf8f6-121">saml2Token</span></span>|<span data-ttu-id="bf8f6-122">[Коллекция optionalClaim](optionalclaim.md)</span><span class="sxs-lookup"><span data-stu-id="bf8f6-122">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="bf8f6-123">Необязательные утверждения, возвращенные в маркере SAML.</span><span class="sxs-lookup"><span data-stu-id="bf8f6-123">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf8f6-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf8f6-124">JSON Representation</span></span>
<span data-ttu-id="bf8f6-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf8f6-125">Here is a JSON representation of the resource.</span></span>
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
