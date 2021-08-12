---
title: Обзор API устройств и приложений Intune
description: 'Microsoft Intune помогает предприятиям управлять устройствами и приложениями в организации. С помощью API Intune в Microsoft Graph вы можете управлять устройствами и приложениями, а также настраивать Intune, используя привычные средства. '
author: dougeby
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 373746111008e627dc066024afa9703794e2e95ee99c048f602578b51e7a64a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205187"
---
# <a name="intune-devices-and-apps-api-overview"></a>Обзор API устройств и приложений Intune

Microsoft Intune помогает предприятиям управлять устройствами и приложениями в организации. С помощью API Intune в Microsoft Graph вы можете управлять устройствами и приложениями, а также настраивать Intune, используя привычные средства. 

Если вы независимый поставщик программного обеспечения, вы также можете использовать API Intune для управления клиентами.

> [!VIDEO https://www.youtube-nocookie.com/embed/yU1HeqNmN7A]

## <a name="why-integrate-with-intune"></a>Преимущества интеграции с Intune

Вы также можете использовать API Intune в Microsoft Graph для доступа к сведениям об устройствах и приложениях из Intune, управления приложениями и автоматизации Intune.

### <a name="manage-devices"></a>Управление устройствами

С помощью API Intune вы можете:

- Определять и применять политики [соответствия устройств различным требованиям](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0), таким как сложность и длина пароля, шифрование, уровни защиты от угроз.  (То, поддерживается ли политика, зависит от используемой операционной системы и ее версии.)
- [Защищать данные компании](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0) независимо от платформы устройства (Windows, Android, Mac или iOS).
- Создавать и развертывать политики [конфигурации устройств](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0), включая платформы и версии операционной системы, членство в доменах и управление параметрами конфигурации.
- Создавать и развертывать политики [контроля доступа](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) для устройств, включая ограниченную загрузку, доступ к сетевым аксессуарам и передачу данных.
- Выполнять [удаленные действия](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), например поиск устройства, изменение пароля и стирание данных устройства.

### <a name="manage-apps"></a>Управление приложениями 

С помощью API Intune вы можете выполнять указанные ниже задачи по управлению приложениями.

- Развертывание [приложений на устройствах](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) и запрет развертывания приложений.
- Управление доступом к [электронным книгам](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) и соответствующим службам.
- Определение и развертывание параметров конфигурации и защиты приложений, а также политик их использования.

### <a name="automate-intune"></a>Автоматизация Intune

Автоматизируйте Intune, используя API Intune для:

- определения и назначения правил доступа [на основе ролей](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0);
- аудита и создания отчетов о соответствии требованиям, использовании и доступе;
- управления [затратами на телекоммуникации](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API Intune в Microsoft Graph 1.0](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [API Intune в бета-версии Microsoft Graph](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

- [Доступ к интерфейсам API Intune в Microsoft Graph с использованием Azure AD](/intune/intune-graph-apis).
- Узнайте, как выполнять распространенные задачи, с помощью [примеров PowerShell для Intune](https://github.com/microsoftgraph/powershell-intune-samples).
- Узнайте, как [использовать REST API Intune](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).
- Сведения о новых возможностях API Intune см. в [журнале изменений](changelog.md).
- Изучите [ресурсы](https://developer.microsoft.com/graph/gallery/) с новыми идеями о том, как использовать Microsoft Graph.