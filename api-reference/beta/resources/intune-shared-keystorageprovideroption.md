---
title: тип перечисления Кэйсторажепровидероптион
description: Параметры импорта поставщика хранилища ключей (KSP).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d0a0fca9dd77a4c83022d875350f12a3e56e18d6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302065"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="24aa9-103">тип перечисления Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="24aa9-103">keyStorageProviderOption enum type</span></span>

<span data-ttu-id="24aa9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24aa9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24aa9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24aa9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24aa9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24aa9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24aa9-107">Параметры импорта поставщика хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="24aa9-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="24aa9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="24aa9-108">Members</span></span>
|<span data-ttu-id="24aa9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="24aa9-109">Member</span></span>|<span data-ttu-id="24aa9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="24aa9-110">Value</span></span>|<span data-ttu-id="24aa9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="24aa9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24aa9-112">усетпмкспосервисеусесофтварексп</span><span class="sxs-lookup"><span data-stu-id="24aa9-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="24aa9-113">нуль</span><span class="sxs-lookup"><span data-stu-id="24aa9-113">0</span></span>|<span data-ttu-id="24aa9-114">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае импортировать в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="24aa9-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="24aa9-115">усетпмкспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="24aa9-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="24aa9-116">1,1</span><span class="sxs-lookup"><span data-stu-id="24aa9-116">1</span></span>|<span data-ttu-id="24aa9-117">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="24aa9-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="24aa9-118">усепасспортфорворккспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="24aa9-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="24aa9-119">2</span><span class="sxs-lookup"><span data-stu-id="24aa9-119">2</span></span>|<span data-ttu-id="24aa9-120">Импорт в паспорт для Works KSP, если он доступен, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="24aa9-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="24aa9-121">усесофтварексп</span><span class="sxs-lookup"><span data-stu-id="24aa9-121">useSoftwareKsp</span></span>|<span data-ttu-id="24aa9-122">4</span><span class="sxs-lookup"><span data-stu-id="24aa9-122">3</span></span>|<span data-ttu-id="24aa9-123">Импорт в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="24aa9-123">Import to Software KSP.</span></span>|




