---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 300243146175c4884c8f8f44691ba02fa796210c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049158"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="d7233-103">тип перечисления Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="d7233-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="d7233-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7233-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7233-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7233-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7233-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7233-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7233-107">Способ проверки подлинности VPN.</span><span class="sxs-lookup"><span data-stu-id="d7233-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="d7233-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d7233-108">Members</span></span>
|<span data-ttu-id="d7233-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d7233-109">Member</span></span>|<span data-ttu-id="d7233-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d7233-110">Value</span></span>|<span data-ttu-id="d7233-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7233-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7233-112">certificate</span><span class="sxs-lookup"><span data-stu-id="d7233-112">certificate</span></span>|<span data-ttu-id="d7233-113">нуль</span><span class="sxs-lookup"><span data-stu-id="d7233-113">0</span></span>|<span data-ttu-id="d7233-114">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="d7233-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="d7233-115">усернамеандпассворд</span><span class="sxs-lookup"><span data-stu-id="d7233-115">usernameAndPassword</span></span>|<span data-ttu-id="d7233-116">1 </span><span class="sxs-lookup"><span data-stu-id="d7233-116">1</span></span>|<span data-ttu-id="d7233-117">Используйте имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d7233-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="d7233-118">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="d7233-118">sharedSecret</span></span>|<span data-ttu-id="d7233-119">2 </span><span class="sxs-lookup"><span data-stu-id="d7233-119">2</span></span>|<span data-ttu-id="d7233-120">Используйте общий секрет для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d7233-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="d7233-121">Поддерживается только для iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="d7233-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="d7233-122">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="d7233-122">derivedCredential</span></span>|<span data-ttu-id="d7233-123">4</span><span class="sxs-lookup"><span data-stu-id="d7233-123">3</span></span>|<span data-ttu-id="d7233-124">Используйте производные учетные данные для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d7233-124">Use Derived Credential for Authentication.</span></span>|
|<span data-ttu-id="d7233-125">azureAD</span><span class="sxs-lookup"><span data-stu-id="d7233-125">azureAD</span></span>|<span data-ttu-id="d7233-126">4 </span><span class="sxs-lookup"><span data-stu-id="d7233-126">4</span></span>|<span data-ttu-id="d7233-127">Используйте Azure AD для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d7233-127">Use Azure AD for authentication.</span></span>|






