---
title: тип перечисления Еапфастконфигуратион
description: Доступные параметры настройки EAP – FAST.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f0d045252c058b2557fd9bb4448e0275953e0b09
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469134"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="b9b9f-103">тип перечисления Еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b9b9f-103">eapFastConfiguration enum type</span></span>

<span data-ttu-id="b9b9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9b9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9b9f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9b9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9b9f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9b9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9b9f-107">Доступные параметры настройки EAP – FAST.</span><span class="sxs-lookup"><span data-stu-id="b9b9f-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="b9b9f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b9b9f-108">Members</span></span>
|<span data-ttu-id="b9b9f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b9b9f-109">Member</span></span>|<span data-ttu-id="b9b9f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b9b9f-110">Value</span></span>|<span data-ttu-id="b9b9f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b9b9f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9b9f-112">нопротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="b9b9f-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="b9b9f-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b9b9f-113">0</span></span>|<span data-ttu-id="b9b9f-114">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="b9b9f-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="b9b9f-115">усепротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="b9b9f-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="b9b9f-116">1,1</span><span class="sxs-lookup"><span data-stu-id="b9b9f-116">1</span></span>|<span data-ttu-id="b9b9f-117">Использование учетных данных безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="b9b9f-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="b9b9f-118">усепротектедакцесскредентиаландпровисион</span><span class="sxs-lookup"><span data-stu-id="b9b9f-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="b9b9f-119">2</span><span class="sxs-lookup"><span data-stu-id="b9b9f-119">2</span></span>|<span data-ttu-id="b9b9f-120">Использование учетных данных безопасного доступа (PAC) и подготовка ключа PAC.</span><span class="sxs-lookup"><span data-stu-id="b9b9f-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="b9b9f-121">усепротектедакцесскредентиаландпровисионанонимаусли</span><span class="sxs-lookup"><span data-stu-id="b9b9f-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="b9b9f-122">4</span><span class="sxs-lookup"><span data-stu-id="b9b9f-122">3</span></span>|<span data-ttu-id="b9b9f-123">Использование учетных данных безопасного доступа (PAC), подготовка ключа PAC и анонимное выполнение.</span><span class="sxs-lookup"><span data-stu-id="b9b9f-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|



