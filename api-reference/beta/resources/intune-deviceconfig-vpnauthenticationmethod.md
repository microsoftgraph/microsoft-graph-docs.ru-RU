---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ef477b17b8ae7e8aedc3b95ce70b66115a3c8712
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123892"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="2d57c-103">тип перечисления Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="2d57c-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="2d57c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d57c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d57c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d57c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d57c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d57c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d57c-107">Способ проверки подлинности VPN.</span><span class="sxs-lookup"><span data-stu-id="2d57c-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="2d57c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2d57c-108">Members</span></span>
|<span data-ttu-id="2d57c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2d57c-109">Member</span></span>|<span data-ttu-id="2d57c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2d57c-110">Value</span></span>|<span data-ttu-id="2d57c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2d57c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d57c-112">certificate</span><span class="sxs-lookup"><span data-stu-id="2d57c-112">certificate</span></span>|<span data-ttu-id="2d57c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2d57c-113">0</span></span>|<span data-ttu-id="2d57c-114">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="2d57c-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="2d57c-115">усернамеандпассворд</span><span class="sxs-lookup"><span data-stu-id="2d57c-115">usernameAndPassword</span></span>|<span data-ttu-id="2d57c-116">1 </span><span class="sxs-lookup"><span data-stu-id="2d57c-116">1</span></span>|<span data-ttu-id="2d57c-117">Используйте имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2d57c-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="2d57c-118">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="2d57c-118">sharedSecret</span></span>|<span data-ttu-id="2d57c-119">2 </span><span class="sxs-lookup"><span data-stu-id="2d57c-119">2</span></span>|<span data-ttu-id="2d57c-120">Используйте общий секрет для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2d57c-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="2d57c-121">Поддерживается только для iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="2d57c-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="2d57c-122">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="2d57c-122">derivedCredential</span></span>|<span data-ttu-id="2d57c-123">3 </span><span class="sxs-lookup"><span data-stu-id="2d57c-123">3</span></span>|<span data-ttu-id="2d57c-124">Используйте производные учетные данные для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2d57c-124">Use Derived Credential for Authentication.</span></span>|
|<span data-ttu-id="2d57c-125">azureAD</span><span class="sxs-lookup"><span data-stu-id="2d57c-125">azureAD</span></span>|<span data-ttu-id="2d57c-126">4 </span><span class="sxs-lookup"><span data-stu-id="2d57c-126">4</span></span>|<span data-ttu-id="2d57c-127">Используйте Azure AD для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2d57c-127">Use Azure AD for authentication.</span></span>|



