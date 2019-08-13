---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58cb031abbcf520a8a970aa80bacd2390b860343
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367794"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="8d360-103">тип перечисления Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="8d360-103">vpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="8d360-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d360-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d360-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d360-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d360-106">Способ проверки подлинности VPN.</span><span class="sxs-lookup"><span data-stu-id="8d360-106">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="8d360-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8d360-107">Members</span></span>
|<span data-ttu-id="8d360-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8d360-108">Member</span></span>|<span data-ttu-id="8d360-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8d360-109">Value</span></span>|<span data-ttu-id="8d360-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8d360-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d360-111">certificate</span><span class="sxs-lookup"><span data-stu-id="8d360-111">certificate</span></span>|<span data-ttu-id="8d360-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8d360-112">0</span></span>|<span data-ttu-id="8d360-113">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="8d360-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="8d360-114">усернамеандпассворд</span><span class="sxs-lookup"><span data-stu-id="8d360-114">usernameAndPassword</span></span>|<span data-ttu-id="8d360-115">1,1</span><span class="sxs-lookup"><span data-stu-id="8d360-115">1</span></span>|<span data-ttu-id="8d360-116">Используйте имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8d360-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="8d360-117">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="8d360-117">sharedSecret</span></span>|<span data-ttu-id="8d360-118">2</span><span class="sxs-lookup"><span data-stu-id="8d360-118">2</span></span>|<span data-ttu-id="8d360-119">Используйте общий секрет для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8d360-119">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="8d360-120">Поддерживается только для iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="8d360-120">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="8d360-121">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="8d360-121">derivedCredential</span></span>|<span data-ttu-id="8d360-122">4</span><span class="sxs-lookup"><span data-stu-id="8d360-122">3</span></span>|<span data-ttu-id="8d360-123">Используйте производные учетные данные для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8d360-123">Use Derived Credential for Authentication.</span></span>  <span data-ttu-id="8d360-124">Поддерживается только для iOS.</span><span class="sxs-lookup"><span data-stu-id="8d360-124">Only valid for iOS.</span></span>|



