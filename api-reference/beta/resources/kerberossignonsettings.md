---
title: Тип ресурса Кербероссигнонсеттингс
description: Представляет параметры Kerberos для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 366a220dc8979c55c95706830d4e3d36a920c130
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401154"
---
# <a name="kerberossignonsettings-resource-type"></a><span data-ttu-id="42828-103">Тип ресурса Кербероссигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="42828-103">kerberosSignOnSettings resource type</span></span>

<span data-ttu-id="42828-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42828-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42828-105">Представляет параметры ограниченного делегирования Кеберос (ККД) для ресурса [онпремисеспублишингсинглесигнон](onpremisespublishingsinglesignon.md) при публикации локального приложения через прокси-сервер приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="42828-105">Represents the Keberos Constrained Delegation (KCD) settings for the [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) resource when publishing an on-premises application via Azure AD Application Proxy.</span></span> <span data-ttu-id="42828-106">Прокси приложения использует ограниченное делегирование Kerberos (ККД) для поддержки единого входа для встроенных приложений проверки подлинности Windows.</span><span class="sxs-lookup"><span data-stu-id="42828-106">Application Proxy uses Kerberos Constrained Delegation (KCD) to support single-sign on to Integrated Windows Authentication applications.</span></span> <span data-ttu-id="42828-107">Дополнительные сведения см. в статье [ограниченное делегирование Kerberos для единого входа в приложения с помощью прокси-сервера приложения](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span><span class="sxs-lookup"><span data-stu-id="42828-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="42828-108">Не используйте это свойство для настройки SAML или единого входа на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="42828-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="42828-109">Если настраивается единый вход SAML, необходимо задать параметр [servicePrincipal](serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="42828-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="42828-110">Если вы настраиваете одиночный символ на основе пароля, его необходимо задать с помощью [креатепассвордсинглесигнонкредентиалс](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span><span class="sxs-lookup"><span data-stu-id="42828-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="42828-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="42828-111">Properties</span></span>

| <span data-ttu-id="42828-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="42828-112">Property</span></span>     | <span data-ttu-id="42828-113">Тип</span><span class="sxs-lookup"><span data-stu-id="42828-113">Type</span></span>        | <span data-ttu-id="42828-114">Описание</span><span class="sxs-lookup"><span data-stu-id="42828-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42828-115">кербероссервицепринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="42828-115">kerberosServicePrincipalName</span></span>|<span data-ttu-id="42828-116">String</span><span class="sxs-lookup"><span data-stu-id="42828-116">String</span></span>| <span data-ttu-id="42828-117">Внутреннее имя субъекта-службы приложения сервера приложений.</span><span class="sxs-lookup"><span data-stu-id="42828-117">The Internal Application SPN of the application server.</span></span> <span data-ttu-id="42828-118">Это имя участника-службы должно быть в списке служб, к которому соединитель может предоставлять делегированные учетные данные.</span><span class="sxs-lookup"><span data-stu-id="42828-118">This SPN needs to be in the list of services to which the connector can present delegated credentials.</span></span> |
|<span data-ttu-id="42828-119">кербероссигнонмаппингаттрибутетипе</span><span class="sxs-lookup"><span data-stu-id="42828-119">kerberosSignOnMappingAttributeType</span></span>|<span data-ttu-id="42828-120">String</span><span class="sxs-lookup"><span data-stu-id="42828-120">String</span></span>| <span data-ttu-id="42828-121">Удостоверение делегированного имени входа для соединителя, которое будет использоваться от имени ваших пользователей.</span><span class="sxs-lookup"><span data-stu-id="42828-121">The Delegated Login Identity for the connector to use on behalf of your users.</span></span> <span data-ttu-id="42828-122">Более подробную информацию можно узнать [в статье работа с другими локальными и облачными удостоверениями ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span><span class="sxs-lookup"><span data-stu-id="42828-122">For more information, see [Working with different on-premises and cloud identities ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span></span> <span data-ttu-id="42828-123">Возможные значения: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span><span class="sxs-lookup"><span data-stu-id="42828-123">Possible values are: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42828-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42828-124">JSON representation</span></span>

<span data-ttu-id="42828-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42828-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.kerberosSignOnSettings",
  "baseType": null
}-->

```json
{
  "kerberosServicePrincipalName": "String",
  "kerberosSignOnMappingAttributeType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "kerberosSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->