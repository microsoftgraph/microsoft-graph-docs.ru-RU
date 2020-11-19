---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3ffc71fa17385ad1e0d00dd77958e65fb7a4aed9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276317"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="18b23-103">тип перечисления Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="18b23-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="18b23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18b23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18b23-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18b23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18b23-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18b23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18b23-107">Способ проверки подлинности VPN.</span><span class="sxs-lookup"><span data-stu-id="18b23-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="18b23-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="18b23-108">Members</span></span>
|<span data-ttu-id="18b23-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="18b23-109">Member</span></span>|<span data-ttu-id="18b23-110">Значение</span><span class="sxs-lookup"><span data-stu-id="18b23-110">Value</span></span>|<span data-ttu-id="18b23-111">Описание</span><span class="sxs-lookup"><span data-stu-id="18b23-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18b23-112">certificate</span><span class="sxs-lookup"><span data-stu-id="18b23-112">certificate</span></span>|<span data-ttu-id="18b23-113">нуль</span><span class="sxs-lookup"><span data-stu-id="18b23-113">0</span></span>|<span data-ttu-id="18b23-114">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="18b23-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="18b23-115">усернамеандпассворд</span><span class="sxs-lookup"><span data-stu-id="18b23-115">usernameAndPassword</span></span>|<span data-ttu-id="18b23-116">1,1</span><span class="sxs-lookup"><span data-stu-id="18b23-116">1</span></span>|<span data-ttu-id="18b23-117">Используйте имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="18b23-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="18b23-118">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="18b23-118">sharedSecret</span></span>|<span data-ttu-id="18b23-119">2</span><span class="sxs-lookup"><span data-stu-id="18b23-119">2</span></span>|<span data-ttu-id="18b23-120">Используйте общий секрет для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="18b23-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="18b23-121">Поддерживается только для iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="18b23-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="18b23-122">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="18b23-122">derivedCredential</span></span>|<span data-ttu-id="18b23-123">4</span><span class="sxs-lookup"><span data-stu-id="18b23-123">3</span></span>|<span data-ttu-id="18b23-124">Используйте производные учетные данные для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="18b23-124">Use Derived Credential for Authentication.</span></span>|
|<span data-ttu-id="18b23-125">azureAD</span><span class="sxs-lookup"><span data-stu-id="18b23-125">azureAD</span></span>|<span data-ttu-id="18b23-126">4 </span><span class="sxs-lookup"><span data-stu-id="18b23-126">4</span></span>|<span data-ttu-id="18b23-127">Используйте Azure AD для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="18b23-127">Use Azure AD for authentication.</span></span>|




