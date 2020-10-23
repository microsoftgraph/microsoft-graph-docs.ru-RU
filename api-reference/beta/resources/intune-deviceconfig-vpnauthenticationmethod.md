---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dbb441bfc32e2de64f5950c033bdd24a3b05c59e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726404"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="c325d-103">тип перечисления Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="c325d-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="c325d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c325d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c325d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c325d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c325d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c325d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c325d-107">Способ проверки подлинности VPN.</span><span class="sxs-lookup"><span data-stu-id="c325d-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="c325d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c325d-108">Members</span></span>
|<span data-ttu-id="c325d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c325d-109">Member</span></span>|<span data-ttu-id="c325d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c325d-110">Value</span></span>|<span data-ttu-id="c325d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c325d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c325d-112">certificate</span><span class="sxs-lookup"><span data-stu-id="c325d-112">certificate</span></span>|<span data-ttu-id="c325d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c325d-113">0</span></span>|<span data-ttu-id="c325d-114">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="c325d-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="c325d-115">усернамеандпассворд</span><span class="sxs-lookup"><span data-stu-id="c325d-115">usernameAndPassword</span></span>|<span data-ttu-id="c325d-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c325d-116">1</span></span>|<span data-ttu-id="c325d-117">Используйте имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c325d-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="c325d-118">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="c325d-118">sharedSecret</span></span>|<span data-ttu-id="c325d-119">2</span><span class="sxs-lookup"><span data-stu-id="c325d-119">2</span></span>|<span data-ttu-id="c325d-120">Используйте общий секрет для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c325d-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="c325d-121">Поддерживается только для iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="c325d-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="c325d-122">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="c325d-122">derivedCredential</span></span>|<span data-ttu-id="c325d-123">4</span><span class="sxs-lookup"><span data-stu-id="c325d-123">3</span></span>|<span data-ttu-id="c325d-124">Используйте производные учетные данные для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c325d-124">Use Derived Credential for Authentication.</span></span>|
|<span data-ttu-id="c325d-125">azureAD</span><span class="sxs-lookup"><span data-stu-id="c325d-125">azureAD</span></span>|<span data-ttu-id="c325d-126">4 </span><span class="sxs-lookup"><span data-stu-id="c325d-126">4</span></span>|<span data-ttu-id="c325d-127">Используйте Azure AD для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c325d-127">Use Azure AD for authentication.</span></span>|





