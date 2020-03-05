---
title: тип перечисления Кэйсторажепровидероптион
description: Параметры импорта поставщика хранилища ключей (KSP).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8580688edbdacb150a37ee5cf2a52fdc77dd490f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526257"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="e0ea0-103">тип перечисления Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="e0ea0-103">keyStorageProviderOption enum type</span></span>

<span data-ttu-id="e0ea0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e0ea0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0ea0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0ea0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0ea0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0ea0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0ea0-107">Параметры импорта поставщика хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="e0ea0-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="e0ea0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e0ea0-108">Members</span></span>
|<span data-ttu-id="e0ea0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e0ea0-109">Member</span></span>|<span data-ttu-id="e0ea0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e0ea0-110">Value</span></span>|<span data-ttu-id="e0ea0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e0ea0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0ea0-112">усетпмкспосервисеусесофтварексп</span><span class="sxs-lookup"><span data-stu-id="e0ea0-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="e0ea0-113">нуль</span><span class="sxs-lookup"><span data-stu-id="e0ea0-113">0</span></span>|<span data-ttu-id="e0ea0-114">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае импортировать в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="e0ea0-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="e0ea0-115">усетпмкспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="e0ea0-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="e0ea0-116">1 </span><span class="sxs-lookup"><span data-stu-id="e0ea0-116">1</span></span>|<span data-ttu-id="e0ea0-117">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="e0ea0-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="e0ea0-118">усепасспортфорворккспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="e0ea0-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="e0ea0-119">2 </span><span class="sxs-lookup"><span data-stu-id="e0ea0-119">2</span></span>|<span data-ttu-id="e0ea0-120">Импорт в паспорт для Works KSP, если он доступен, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="e0ea0-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="e0ea0-121">усесофтварексп</span><span class="sxs-lookup"><span data-stu-id="e0ea0-121">useSoftwareKsp</span></span>|<span data-ttu-id="e0ea0-122">3 </span><span class="sxs-lookup"><span data-stu-id="e0ea0-122">3</span></span>|<span data-ttu-id="e0ea0-123">Импорт в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="e0ea0-123">Import to Software KSP.</span></span>|



