---
title: Тип ресурса kerberosSignOnSettings
description: Представляет параметры единого знака для локального приложения, опубликованного через прокси-сервер приложения.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 85b2b4963c077b8dcb6ded4818ecc57bce635b39
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134871"
---
# <a name="onpremisespublishingsinglesignon-resource-type"></a><span data-ttu-id="a6935-103">Тип ресурса onPremisesPublishingSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="a6935-103">onPremisesPublishingSingleSignOn resource type</span></span>

<span data-ttu-id="a6935-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6935-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6935-105">Представляет параметры единого входов для ресурса [onPremisesPublishing](onpremisespublishing.md) при публикации локального приложения с помощью прокси приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a6935-105">Represents the single sign-on settings for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Azure AD Application Proxy.</span></span> <span data-ttu-id="a6935-106">Этот ресурс используется для настройки встроенной проверки подлинности Windows и проверки подлинности на основе загона в режиме единого входов.</span><span class="sxs-lookup"><span data-stu-id="a6935-106">This resource is used for setting Integrated Windows Authentication and header-based authentication as the single-sign on mode.</span></span> <span data-ttu-id="a6935-107">Дополнительные сведения см. в сведениях о ограниченном делегирования [Kerberos](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)для единого вход в приложения с помощью прокси приложения.</span><span class="sxs-lookup"><span data-stu-id="a6935-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="a6935-108">Не используйте это свойство для настройки SAML или единого вход на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="a6935-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="a6935-109">Если вы настраиваете единый вход SAML, это должно быть установлено в [servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="a6935-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="a6935-110">Если вы настраиваете единый знак на основе пароля, его необходимо настроить с помощью [createPasswordSingleSignOnCredentials.](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)</span><span class="sxs-lookup"><span data-stu-id="a6935-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a6935-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6935-111">Properties</span></span>

| <span data-ttu-id="a6935-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6935-112">Property</span></span>     | <span data-ttu-id="a6935-113">Тип</span><span class="sxs-lookup"><span data-stu-id="a6935-113">Type</span></span>        | <span data-ttu-id="a6935-114">Описание</span><span class="sxs-lookup"><span data-stu-id="a6935-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a6935-115">kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="a6935-115">kerberosSignOnSettings</span></span>| [<span data-ttu-id="a6935-116">kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="a6935-116">kerberosSignOnSettings</span></span>](kerberossignonsettings.md)| <span data-ttu-id="a6935-117">Параметры ограниченного делегирования Kerberos для приложений, которые используют встроенную проверку подлинности окон.</span><span class="sxs-lookup"><span data-stu-id="a6935-117">The Kerberos Constrained Delegation settings for applications that use Integrated Window Authentication.</span></span> |
|<span data-ttu-id="a6935-118">singleSignOnMode</span><span class="sxs-lookup"><span data-stu-id="a6935-118">singleSignOnMode</span></span>|<span data-ttu-id="a6935-119">Строка</span><span class="sxs-lookup"><span data-stu-id="a6935-119">String</span></span>| <span data-ttu-id="a6935-120">Предпочтительный режим единого входов для приложения.</span><span class="sxs-lookup"><span data-stu-id="a6935-120">The preferred single-sign on mode for the application.</span></span> <span data-ttu-id="a6935-121">Возможные значения: `none`, `onPremisesKerberos`, `headerBased`.</span><span class="sxs-lookup"><span data-stu-id="a6935-121">Possible values are: `none`, `onPremisesKerberos`, `headerBased`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6935-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a6935-122">JSON representation</span></span>

<span data-ttu-id="a6935-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6935-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn",
  "baseType": null
}-->

```json
{
  "kerberosSignOnSettings": {"@odata.type": "microsoft.graph.kerberosSignOnSettings"},
  "singleSignOnMode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingSingleSignOn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
