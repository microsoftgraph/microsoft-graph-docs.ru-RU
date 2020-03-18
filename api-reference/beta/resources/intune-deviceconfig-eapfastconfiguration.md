---
title: тип перечисления Еапфастконфигуратион
description: Доступные параметры настройки EAP – FAST.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b70e2688473f9af93dcd3b0f0d4d05b77d81446f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791956"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="17a55-103">тип перечисления Еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="17a55-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="17a55-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17a55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17a55-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17a55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17a55-106">Доступные параметры настройки EAP – FAST.</span><span class="sxs-lookup"><span data-stu-id="17a55-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="17a55-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="17a55-107">Members</span></span>
|<span data-ttu-id="17a55-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="17a55-108">Member</span></span>|<span data-ttu-id="17a55-109">Значение</span><span class="sxs-lookup"><span data-stu-id="17a55-109">Value</span></span>|<span data-ttu-id="17a55-110">Описание</span><span class="sxs-lookup"><span data-stu-id="17a55-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17a55-111">нопротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="17a55-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="17a55-112">нуль</span><span class="sxs-lookup"><span data-stu-id="17a55-112">0</span></span>|<span data-ttu-id="17a55-113">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="17a55-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="17a55-114">усепротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="17a55-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="17a55-115">1,1</span><span class="sxs-lookup"><span data-stu-id="17a55-115">1</span></span>|<span data-ttu-id="17a55-116">Использование учетных данных безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="17a55-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="17a55-117">усепротектедакцесскредентиаландпровисион</span><span class="sxs-lookup"><span data-stu-id="17a55-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="17a55-118">2</span><span class="sxs-lookup"><span data-stu-id="17a55-118">2</span></span>|<span data-ttu-id="17a55-119">Использование учетных данных безопасного доступа (PAC) и подготовка ключа PAC.</span><span class="sxs-lookup"><span data-stu-id="17a55-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="17a55-120">усепротектедакцесскредентиаландпровисионанонимаусли</span><span class="sxs-lookup"><span data-stu-id="17a55-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="17a55-121">4</span><span class="sxs-lookup"><span data-stu-id="17a55-121">3</span></span>|<span data-ttu-id="17a55-122">Использование учетных данных безопасного доступа (PAC), подготовка ключа PAC и анонимное выполнение.</span><span class="sxs-lookup"><span data-stu-id="17a55-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|



