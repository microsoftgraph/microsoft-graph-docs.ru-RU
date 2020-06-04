---
title: Тип ресурса Кербероссигнонсеттингс
description: Представляет параметры единого входа для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f07fc81fee6fdc8e8ff3b55c246facdc4f155d11
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556444"
---
# <a name="onpremisespublishingsinglesignon-resource-type"></a><span data-ttu-id="2c1b9-103">Тип ресурса Онпремисеспублишингсинглесигнон</span><span class="sxs-lookup"><span data-stu-id="2c1b9-103">onPremisesPublishingSingleSignOn resource type</span></span>

<span data-ttu-id="2c1b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c1b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c1b9-105">Представляет параметры единого входа для ресурса [онпремисеспублишинг](onpremisespublishing.md) при публикации локального приложения с помощью прокси приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2c1b9-105">Represents the single sign-on settings for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Azure AD Application Proxy.</span></span> <span data-ttu-id="2c1b9-106">Этот ресурс используется для настройки встроенной проверки подлинности Windows и проверки подлинности на основе заголовков в режиме единого входа.</span><span class="sxs-lookup"><span data-stu-id="2c1b9-106">This resource is used for setting Integrated Windows Authentication and header-based authentication as the single-sign on mode.</span></span> <span data-ttu-id="2c1b9-107">Дополнительные сведения см. в статье [ограниченное делегирование Kerberos для единого входа в приложения с помощью прокси-сервера приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span><span class="sxs-lookup"><span data-stu-id="2c1b9-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="2c1b9-108">Не используйте это свойство для настройки SAML или единого входа на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="2c1b9-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="2c1b9-109">Если настраивается единый вход SAML, необходимо задать параметр [servicePrincipal](serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="2c1b9-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="2c1b9-110">Если вы настраиваете одиночный символ на основе пароля, его необходимо задать с помощью [креатепассвордсинглесигнонкредентиалс](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span><span class="sxs-lookup"><span data-stu-id="2c1b9-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2c1b9-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c1b9-111">Properties</span></span>

| <span data-ttu-id="2c1b9-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c1b9-112">Property</span></span>     | <span data-ttu-id="2c1b9-113">Тип</span><span class="sxs-lookup"><span data-stu-id="2c1b9-113">Type</span></span>        | <span data-ttu-id="2c1b9-114">Описание</span><span class="sxs-lookup"><span data-stu-id="2c1b9-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c1b9-115">кербероссигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="2c1b9-115">kerberosSignOnSettings</span></span>| [<span data-ttu-id="2c1b9-116">кербероссигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="2c1b9-116">kerberosSignOnSettings</span></span>](kerberossignonsettings.md)| <span data-ttu-id="2c1b9-117">Параметры ограниченного делегирования Kerberos для приложения.</span><span class="sxs-lookup"><span data-stu-id="2c1b9-117">The Kerberos Constrained Delegation settings for the application.</span></span> |
|<span data-ttu-id="2c1b9-118">синглесигнонмоде</span><span class="sxs-lookup"><span data-stu-id="2c1b9-118">singleSignOnMode</span></span>|<span data-ttu-id="2c1b9-119">String</span><span class="sxs-lookup"><span data-stu-id="2c1b9-119">String</span></span>| <span data-ttu-id="2c1b9-120">Предпочтительный режим единого входа для приложения.</span><span class="sxs-lookup"><span data-stu-id="2c1b9-120">The preferred single-sign on mode for the application.</span></span> <span data-ttu-id="2c1b9-121">Возможные значения: `none`, `onPremisesKerberos`, `headerBased`.</span><span class="sxs-lookup"><span data-stu-id="2c1b9-121">Possible values are: `none`, `onPremisesKerberos`, `headerBased`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c1b9-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c1b9-122">JSON representation</span></span>

<span data-ttu-id="2c1b9-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c1b9-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn",
  "baseType": null
}-->

```json
{
  "KerberosSignOnSettings": {"@odata.type": "microsoft.graph.kerberosSignOnSettings"},
  "SingleSignOnMode": "String"
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