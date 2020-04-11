---
title: Общие сведения об API политики
description: Azure Active Directory использует политики для управления поведением компонентов Azure AD в вашей организации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: b64efc81caa10c249030e33cb893d90aec8a1afb
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229446"
---
# <a name="azure-ad-policy-overview"></a><span data-ttu-id="f6814-103">Общие сведения о политике Azure AD</span><span class="sxs-lookup"><span data-stu-id="f6814-103">Azure AD policy overview</span></span>

<span data-ttu-id="f6814-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6814-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="f6814-105">Azure Active Directory (Azure AD) использует политики для управления поведением компонентов Azure AD в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="f6814-105">Azure Active Directory (Azure AD) uses policies to control Azure AD feature behaviors in your organization.</span></span> <span data-ttu-id="f6814-106">Политики это настраиваемые правила, которые можно применять к приложениям, субъектам, группам или всем организациям, которым они назначены.</span><span class="sxs-lookup"><span data-stu-id="f6814-106">Policies are custom rules that you can enforce on applications, service principals, groups, or on the entire organization they are assigned to.</span></span>

## <a name="what-policies-are-available"></a><span data-ttu-id="f6814-107">Какие политики доступны?</span><span class="sxs-lookup"><span data-stu-id="f6814-107">What policies are available?</span></span>

| <span data-ttu-id="f6814-108">Тип политики</span><span class="sxs-lookup"><span data-stu-id="f6814-108">Policy type</span></span>       | <span data-ttu-id="f6814-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f6814-109">Description</span></span> | <span data-ttu-id="f6814-110">Примеры</span><span class="sxs-lookup"><span data-stu-id="f6814-110">Examples</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="f6814-111">activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="f6814-111">activityBasedTimeoutPolicies</span></span>](activityBasedTimeoutPolicy.md)| <span data-ttu-id="f6814-112">Представляет политику, которая управляет автоматическим выходом для веб-сеансов после определенного периода бездействия для приложений, поддерживающих функции времени ожидания на основе действий.</span><span class="sxs-lookup"><span data-stu-id="f6814-112">Represents a policy that controls automatic sign-out for web sessions after a period of inactivity, for applications that support activity-based timeout functionality.</span></span>| <span data-ttu-id="f6814-113">Настройте на портале Azure время ожидания простоя в 15 минут.</span><span class="sxs-lookup"><span data-stu-id="f6814-113">Configure the Azure portal to have an inactivity timeout of 15 minutes.</span></span> |
|[<span data-ttu-id="f6814-114">homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="f6814-114">homeRealmDiscoveryPolicies</span></span>](homeRealmDiscoveryPolicy.md)| <span data-ttu-id="f6814-115">Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федеративных доменах.</span><span class="sxs-lookup"><span data-stu-id="f6814-115">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span>| <span data-ttu-id="f6814-116">Настройте все пользователи для пропуска обнаружения домашней области и маршрутизации непосредственно в ADFS для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f6814-116">Configure all users to skip home realm discovery and be routed directly to ADFS for authentication.</span></span> |
|[<span data-ttu-id="f6814-117">tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="f6814-117">tokenLifetimePolicies</span></span>](tokenlifetimepolicy.md)|<span data-ttu-id="f6814-118">Представляет срок жизни маркеров доступа, используемых для доступа к защищенным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="f6814-118">Represents the lifetime duration of access tokens used to access protected resources.</span></span>| <span data-ttu-id="f6814-119">Настройка особенно конфиденциального приложения с использованием более короткого срока действия маркера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6814-119">Configure a particularly sensitive application with a shorter than default token lifetime.</span></span>|
|[<span data-ttu-id="f6814-120">токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="f6814-120">tokenIssuancePolicy</span></span>](tokenIssuancePolicy.md)|<span data-ttu-id="f6814-121">Представляет политику, определяющую характеристики маркеров SAML, выданных Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f6814-121">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span>| <span data-ttu-id="f6814-122">Настройте алгоритм подписи или версию токена SAML, которые будут использоваться для выдачи маркера SAML.</span><span class="sxs-lookup"><span data-stu-id="f6814-122">Configure the signing algorithm or SAML token version to be used to issue the SAML token.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f6814-123">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f6814-123">Next steps</span></span>

* <span data-ttu-id="f6814-124">Просмотрите различные типы ресурсов политики, перечисленные выше, и их различные методы.</span><span class="sxs-lookup"><span data-stu-id="f6814-124">Review the different policy resouce types listed above and their various methods.</span></span>
* <span data-ttu-id="f6814-125">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="f6814-125">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
