---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 20374a3008e84b00ce7622019f4a3b8306a07318
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969522"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="ff35c-103">тип перечисления Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="ff35c-103">vpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="ff35c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff35c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff35c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff35c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff35c-106">Способ проверки подлинности VPN.</span><span class="sxs-lookup"><span data-stu-id="ff35c-106">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="ff35c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ff35c-107">Members</span></span>
|<span data-ttu-id="ff35c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ff35c-108">Member</span></span>|<span data-ttu-id="ff35c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ff35c-109">Value</span></span>|<span data-ttu-id="ff35c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff35c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff35c-111">certificate</span><span class="sxs-lookup"><span data-stu-id="ff35c-111">certificate</span></span>|<span data-ttu-id="ff35c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ff35c-112">0</span></span>|<span data-ttu-id="ff35c-113">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="ff35c-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="ff35c-114">Усернамеандпассворд</span><span class="sxs-lookup"><span data-stu-id="ff35c-114">usernameAndPassword</span></span>|<span data-ttu-id="ff35c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ff35c-115">1</span></span>|<span data-ttu-id="ff35c-116">Используйте имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ff35c-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="ff35c-117">Шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="ff35c-117">sharedSecret</span></span>|<span data-ttu-id="ff35c-118">2</span><span class="sxs-lookup"><span data-stu-id="ff35c-118">2</span></span>|<span data-ttu-id="ff35c-119">Используйте общий секрет для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ff35c-119">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="ff35c-120">Поддерживается только для iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="ff35c-120">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="ff35c-121">Дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="ff35c-121">derivedCredential</span></span>|<span data-ttu-id="ff35c-122">4</span><span class="sxs-lookup"><span data-stu-id="ff35c-122">3</span></span>|<span data-ttu-id="ff35c-123">Используйте производные учетные данные для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ff35c-123">Use Derived Credential for Authentication.</span></span>  <span data-ttu-id="ff35c-124">Поддерживается только для iOS.</span><span class="sxs-lookup"><span data-stu-id="ff35c-124">Only valid for iOS.</span></span>|





