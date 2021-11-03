---
title: Работа с Windows 365 облачными компьютерами с помощью API microsoft Graph
description: С помощью microsoft Graph вы можете продюсировать и управлять облачными компьютерами в организации, а если они будут использоваться совместно с API Intune, вы сможете управлять облачными компьютерами наряду с физическими конечными точками.
author: cohanley
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e4e205631424ed2f93b748371c8f32c31b4398ee
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695428"
---
# <a name="working-with-windows-365-cloud-pcs-using-the-microsoft-graph-api"></a>Работа с Windows 365 облачными компьютерами с помощью API microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows 365 — это облачная служба, которая содержит и содержит облачные КОМПЬЮТЕРы в качестве виртуальных машин для конечных пользователей. Администраторы могут легко настроить, управлять и масштабировать Windows 365 облачных КОМПЬЮТЕРов, чтобы соответствовать потребностям организации. Отдельные конечные пользователи могут безопасно передавать свои богатые и персонализированные Windows, включая приложения, данные, контент и параметры, из облака Майкрософт на любое устройство в любое время с Windows 365 cloud PC.

API microsoft Graph программный доступ к сведениям о облачных КОМПЬЮТЕРАх и действиям по управлению в организации. API выполняет те же операции, что и доступные через Microsoft Endpoint Manager. 

> [!IMPORTANT]
> Для использования API Graph Microsoft для облачных компьютеров требуется активная лицензия [Windows 365](https://www.microsoft.com/windows-365) для организации. В настоящее время API Graph Microsoft доступен для Windows 365 Enterprise и не Windows 365 Business. 

## <a name="using-the-microsoft-graph-api-for-cloud-pcs"></a>Использование API Graph Microsoft для облачных компьютеров

С помощью microsoft Graph вы можете закадровку и управление облачными компьютерами в вашей организации. Если используется совместно с API Intune, вы также можете управлять облачными компьютерами наряду с физическими конечными точками. 

## <a name="using-microsoft-graph-permissions"></a>Использование разрешений Microsoft Graph

Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения. Как разработчик необходимо указать разрешения, необходимые для доступа Windows 365 ресурсов. Как правило, разрешения указываются на портале Azure Active Directory. Дополнительные сведения см. в [статье Microsoft Graph разрешений и](/graph/permissions-reference) перейдите в раздел Разрешения облачных [ПК.](/graph/permissions-reference#cloud-pc-permissions) 

## <a name="common-use-cases"></a>Основные варианты использования

|Варианты использования|Ресурсы REST|См. также|
|:---|:---|:---|
|Список, создание, обновление, удаление или назначение политик провизии|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|[Обзор подготовка](/windows-365/enterprise/provisioning)|
|Управление облачными компьютерами, включая перепроизводение, конечный период льготы для облачных ПК, массовое перепроизводение и повторное создание облачных компьютеров|[cloudPC](../resources/cloudpc.md)|[Жизненный цикл облачных компьютеров](/windows-365/enterprise/lifecycle)|
|Список, получить, создать, удалить, получить исходные изображения и перезагрузить изображения облачной ОС ПК|[cloudPCDeviceImage](../resources/cloudpcdeviceimage.md)|[Обзор изображений устройств](/windows-365/enterprise/device-images)|
|Список, создание, удаление, обновление, обновление пароля домена AD и проверка состояния локальной сети|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|[Обзор локального сетевого подключения](/windows-365/enterprise/on-premises-network-connections)|
|Список событий аудита для облачных компьютеров, получения определенного события аудита и получения типов действий аудита|[cloudPcAuditEvent](../resources/cloudpcauditevent.md)|[Получить журналы аудита облачных ПК](/windows-365/enterprise/get-cloud-pc-audit-logs-using-powershell)|
|Список, получить, создать, обновить, удалить или назначить параметры пользователей|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|[Обзор параметров пользователей](../resources/cloudpcusersetting.md)|

## <a name="whats-new"></a>Новые возможности

Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.