---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 048b31bd835c1e94d3afcef87b6bd8e93f3ddeec
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787420"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="5e2da-103">тип перечисления Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="5e2da-103">vpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="5e2da-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e2da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e2da-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e2da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e2da-106">Способ проверки подлинности VPN.</span><span class="sxs-lookup"><span data-stu-id="5e2da-106">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="5e2da-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5e2da-107">Members</span></span>
|<span data-ttu-id="5e2da-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5e2da-108">Member</span></span>|<span data-ttu-id="5e2da-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5e2da-109">Value</span></span>|<span data-ttu-id="5e2da-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5e2da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e2da-111">certificate</span><span class="sxs-lookup"><span data-stu-id="5e2da-111">certificate</span></span>|<span data-ttu-id="5e2da-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5e2da-112">0</span></span>|<span data-ttu-id="5e2da-113">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="5e2da-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="5e2da-114">усернамеандпассворд</span><span class="sxs-lookup"><span data-stu-id="5e2da-114">usernameAndPassword</span></span>|<span data-ttu-id="5e2da-115">1,1</span><span class="sxs-lookup"><span data-stu-id="5e2da-115">1</span></span>|<span data-ttu-id="5e2da-116">Используйте имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5e2da-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="5e2da-117">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="5e2da-117">sharedSecret</span></span>|<span data-ttu-id="5e2da-118">2</span><span class="sxs-lookup"><span data-stu-id="5e2da-118">2</span></span>|<span data-ttu-id="5e2da-119">Используйте общий секрет для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5e2da-119">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="5e2da-120">Поддерживается только для iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="5e2da-120">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="5e2da-121">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="5e2da-121">derivedCredential</span></span>|<span data-ttu-id="5e2da-122">4</span><span class="sxs-lookup"><span data-stu-id="5e2da-122">3</span></span>|<span data-ttu-id="5e2da-123">Используйте производные учетные данные для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5e2da-123">Use Derived Credential for Authentication.</span></span>|



