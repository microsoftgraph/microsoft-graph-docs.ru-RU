---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 343b8e3809a3f61926521a43d873161b2d5eee5f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994316"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="d2790-103">тип перечисления Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="d2790-103">vpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="d2790-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2790-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2790-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2790-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2790-106">Способ проверки подлинности VPN.</span><span class="sxs-lookup"><span data-stu-id="d2790-106">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="d2790-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d2790-107">Members</span></span>
|<span data-ttu-id="d2790-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d2790-108">Member</span></span>|<span data-ttu-id="d2790-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d2790-109">Value</span></span>|<span data-ttu-id="d2790-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d2790-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2790-111">certificate</span><span class="sxs-lookup"><span data-stu-id="d2790-111">certificate</span></span>|<span data-ttu-id="d2790-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d2790-112">0</span></span>|<span data-ttu-id="d2790-113">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="d2790-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="d2790-114">Усернамеандпассворд</span><span class="sxs-lookup"><span data-stu-id="d2790-114">usernameAndPassword</span></span>|<span data-ttu-id="d2790-115">1,1</span><span class="sxs-lookup"><span data-stu-id="d2790-115">1</span></span>|<span data-ttu-id="d2790-116">Используйте имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d2790-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="d2790-117">Шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="d2790-117">sharedSecret</span></span>|<span data-ttu-id="d2790-118">2</span><span class="sxs-lookup"><span data-stu-id="d2790-118">2</span></span>|<span data-ttu-id="d2790-119">Используйте общий секрет для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d2790-119">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="d2790-120">Поддерживается только для iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="d2790-120">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="d2790-121">Дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="d2790-121">derivedCredential</span></span>|<span data-ttu-id="d2790-122">4</span><span class="sxs-lookup"><span data-stu-id="d2790-122">3</span></span>|<span data-ttu-id="d2790-123">Используйте производные учетные данные для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d2790-123">Use Derived Credential for Authentication.</span></span>  <span data-ttu-id="d2790-124">Поддерживается только для iOS.</span><span class="sxs-lookup"><span data-stu-id="d2790-124">Only valid for iOS.</span></span>|





