---
title: тип перечисления Кэйсторажепровидероптион
description: Параметры импорта поставщика хранилища ключей (KSP).
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1d3098daf1d2baf30788328e8cf5c5f665029ab0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439954"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="2ab80-103">тип перечисления Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="2ab80-103">keyStorageProviderOption enum type</span></span>

<span data-ttu-id="2ab80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ab80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ab80-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ab80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ab80-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ab80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ab80-107">Параметры импорта поставщика хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="2ab80-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="2ab80-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2ab80-108">Members</span></span>
|<span data-ttu-id="2ab80-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2ab80-109">Member</span></span>|<span data-ttu-id="2ab80-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2ab80-110">Value</span></span>|<span data-ttu-id="2ab80-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2ab80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab80-112">усетпмкспосервисеусесофтварексп</span><span class="sxs-lookup"><span data-stu-id="2ab80-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="2ab80-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2ab80-113">0</span></span>|<span data-ttu-id="2ab80-114">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае импортировать в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="2ab80-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="2ab80-115">усетпмкспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="2ab80-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="2ab80-116">1,1</span><span class="sxs-lookup"><span data-stu-id="2ab80-116">1</span></span>|<span data-ttu-id="2ab80-117">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="2ab80-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="2ab80-118">усепасспортфорворккспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="2ab80-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="2ab80-119">2</span><span class="sxs-lookup"><span data-stu-id="2ab80-119">2</span></span>|<span data-ttu-id="2ab80-120">Импорт в паспорт для Works KSP, если он доступен, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="2ab80-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="2ab80-121">усесофтварексп</span><span class="sxs-lookup"><span data-stu-id="2ab80-121">useSoftwareKsp</span></span>|<span data-ttu-id="2ab80-122">4</span><span class="sxs-lookup"><span data-stu-id="2ab80-122">3</span></span>|<span data-ttu-id="2ab80-123">Импорт в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="2ab80-123">Import to Software KSP.</span></span>|



