---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dd3cc6887f5434df00a2ed9a817c0ca79c8c880e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412453"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="4a291-103">тип перечисления Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="4a291-103">vpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="4a291-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a291-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a291-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a291-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a291-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a291-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a291-107">Способ проверки подлинности VPN.</span><span class="sxs-lookup"><span data-stu-id="4a291-107">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="4a291-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4a291-108">Members</span></span>
|<span data-ttu-id="4a291-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4a291-109">Member</span></span>|<span data-ttu-id="4a291-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4a291-110">Value</span></span>|<span data-ttu-id="4a291-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4a291-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a291-112">certificate</span><span class="sxs-lookup"><span data-stu-id="4a291-112">certificate</span></span>|<span data-ttu-id="4a291-113">нуль</span><span class="sxs-lookup"><span data-stu-id="4a291-113">0</span></span>|<span data-ttu-id="4a291-114">Проверка подлинности с помощью сертификата.</span><span class="sxs-lookup"><span data-stu-id="4a291-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="4a291-115">усернамеандпассворд</span><span class="sxs-lookup"><span data-stu-id="4a291-115">usernameAndPassword</span></span>|<span data-ttu-id="4a291-116">1,1</span><span class="sxs-lookup"><span data-stu-id="4a291-116">1</span></span>|<span data-ttu-id="4a291-117">Используйте имя пользователя и пароль для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="4a291-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="4a291-118">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="4a291-118">sharedSecret</span></span>|<span data-ttu-id="4a291-119">2</span><span class="sxs-lookup"><span data-stu-id="4a291-119">2</span></span>|<span data-ttu-id="4a291-120">Используйте общий секрет для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="4a291-120">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="4a291-121">Поддерживается только для iOS IKEv2.</span><span class="sxs-lookup"><span data-stu-id="4a291-121">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="4a291-122">дериведкредентиал</span><span class="sxs-lookup"><span data-stu-id="4a291-122">derivedCredential</span></span>|<span data-ttu-id="4a291-123">4</span><span class="sxs-lookup"><span data-stu-id="4a291-123">3</span></span>|<span data-ttu-id="4a291-124">Используйте производные учетные данные для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="4a291-124">Use Derived Credential for Authentication.</span></span>|



