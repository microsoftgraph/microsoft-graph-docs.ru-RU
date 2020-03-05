---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 035fe88bbcde357fd67c42252c6e903f1c610275
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525798"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="cce78-103">тип перечисления Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="cce78-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="cce78-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cce78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cce78-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cce78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cce78-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cce78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cce78-107">Способ проверки подлинности VPN.</span><span class="sxs-lookup"><span data-stu-id="cce78-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="cce78-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="cce78-108">Members</span></span>
|<span data-ttu-id="cce78-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="cce78-109">Member</span></span>|<span data-ttu-id="cce78-110">Значение</span><span class="sxs-lookup"><span data-stu-id="cce78-110">Value</span></span>|<span data-ttu-id="cce78-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cce78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cce78-112">certificate</span><span class="sxs-lookup"><span data-stu-id="cce78-112">certificate</span></span>|<span data-ttu-id="cce78-113">нуль</span><span class="sxs-lookup"><span data-stu-id="cce78-113">0</span></span>|<span data-ttu-id="cce78-114">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="cce78-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="cce78-115">усернамеандпассворд</span><span class="sxs-lookup"><span data-stu-id="cce78-115">usernameAndPassword</span></span>|<span data-ttu-id="cce78-116">1 </span><span class="sxs-lookup"><span data-stu-id="cce78-116">1</span></span>|<span data-ttu-id="cce78-117">Используйте имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="cce78-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="cce78-118">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="cce78-118">sharedSecret</span></span>|<span data-ttu-id="cce78-119">2 </span><span class="sxs-lookup"><span data-stu-id="cce78-119">2</span></span>|<span data-ttu-id="cce78-120">Используйте общий секрет для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="cce78-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="cce78-121">Поддерживается только для iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="cce78-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="cce78-122">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="cce78-122">derivedCredential</span></span>|<span data-ttu-id="cce78-123">3 </span><span class="sxs-lookup"><span data-stu-id="cce78-123">3</span></span>|<span data-ttu-id="cce78-124">Используйте производные учетные данные для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="cce78-124">Use Derived Credential for Authentication.</span></span>|



