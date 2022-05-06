---
title: Наборы данных, регионы и приемники, поддерживаемые подключением к данным Microsoft Graph
description: Описаны поддерживаемые наборы данных и типы конечных хранилищ, которые можно использовать с подключением к данным Microsoft Graph.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: 6d73482dbf2b8b0c85851970460836094a982ad3
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247197"
---
# <a name="datasets-regions-and-sinks-supported-by-microsoft-graph-data-connect"></a>Наборы данных, регионы и приемники, поддерживаемые подключением к данным Microsoft Graph

Подключение к данным Microsoft Graph поддерживает разные наборы данных, регионы данных и места хранения в Microsoft Azure. В этой статье описываются поддерживаемые наборы данных и способы доступа к схемам наборов данных, поддерживаемые регионы Microsoft 365 и Microsoft Azure, а также места хранения, которые Data Connect использует через фабрику данных Azure.

## <a name="datasets"></a>Наборы данных

Microsoft Graph Data Connect сейчас поддерживает следующие наборы данных. Чтобы просмотреть схемы для каждого набора данных, создайте новый набор данных в фабрике данных Azure и используйте вкладку ''Схема'' для его просмотра.

| Имя набора данных | Описание | Пример | Схема |
|--------------|-------------|--------|--------|
| BasicDataSet_v0.CalendarView_v0    | Содержит события из представления календаря.                                        | [CalendarView_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.CalendarView_v0.json)      | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/CalendarView_v0.md) |
| BasicDataSet_v0.Contact_v0         | Содержит доступные сведения из адресной книги каждого пользователя.                  | [Contact_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Contact_v0.json)                | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Contact_v0.md) |
| BasicDataSet_v0.Contact_v1         | Содержит контактные данные из адресной книги каждого пользователя.                        | [Contact_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Contact_v1.json)                | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Contact_v1.md) |
| BasicDataSet_v0.DirectReport_v0    | Содержит сведения о сотрудниках, находящихся в непосредственном подчинении каждого пользователя.   | [DirectReport_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.DirectReport_v0.json)      | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/DirectReport_v0.md) |
| BasicDataSet_v0.Event_v0           | Содержит сведения из событий календаря пользователя.                            | [Event_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Event_v0.json)                    | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Event_v0.md) |
| BasicDataSet_v0.Event_v1           | Содержит события из календаря каждого пользователя.                                       | [Event_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Event_v1.json)                    | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Event_v1.md) |
| BasicDataSet_v0.Inbox_v1      | Содержит папки почты из папки "Входящие" каждого пользователя.                                | [Inbox_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Inbox_v1.json)          | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Inbox_v1.md) |
| BasicDataSet_v0.MailboxSettings_v0 | Содержит параметры почтового ящика каждого пользователя.                                        | [MailboxSetting_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.MailboxSettings_v0.json) | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/MailboxSettings_v0.md) |
| BasicDataSet_v0.MailFolder_v0      | Содержит папки почты из почтового ящика каждого пользователя.                                | [MailFolder_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.MailFolder_v0.json)          | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/MailFolder_v0.md) |
| BasicDataSet_v0.Manager_v0         | Содержит сведения о пользователе для руководителя каждого пользователя.                            | [Manager_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Manager_v0.json)                | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Manager_v0.md) |
| BasicDataSet_v0.Message_v0         | Содержит сообщения электронной почты из почтового ящика пользователя.                                       | [Message_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Message_v0.json)                | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Message_v0.md) |
| BasicDataSet_v0.Message_v1         | Содержит сообщение электронной почты из почтового ящика каждого пользователя.                                       | [Message_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Message_v1.json)                | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Message_v1.md) |
| BasicDataSet_v0.SentItem_v0        | Содержит сообщения, отправленные из почтового ящика каждого пользователя.                               | [SentItem_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.SentItem_v0.json)              | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/SentItem_v0.md) |
| BasicDataSet_v0.SentItem_v1        | Содержит сообщение, отправленное из почтового ящика каждого пользователя.                                | [SentItem_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.SentItem_v1.json)              | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/SentItem_v1.md) |
| BasicDataSet_v0.TeamChat_v1        | Содержит [сообщения чата Teams](https://support.microsoft.com/office/first-things-to-know-about-chat-in-microsoft-teams-88ed0a06-6b59-43a3-8cf7-40c01f2f92f2) для личных и групповых чатов. Этот набор данных исключает сообщения чата, явно удаленные пользователями.     | [TeamChat_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.TeamChat_v1.json)              | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/TeamChat_v1.md) |
| BasicDataSet_v0.User_v0            | Содержит сведения о пользователе (DisplayName, UserPrincipalName и другую информацию). | [User_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.User_v0.json)                      | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/User_v0.md) |
| BasicDataSet_v0.User_v1            | Содержит сведения о пользователе.                                                         | [User_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.User_v1.json)                      | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/User_v1.md) |
| DocumentSharingDataset_v0_Preview            | Содержит сведения о разрешении общего доступа к документам.                                                         | [DocumentSharingDataset_v0_Preview](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/DocumentSharingDataset_v0_Preview.json)                      | [Схема](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/DocumentSharingDataset_v0_Preview.md) |

## <a name="regions"></a>Регионы

Microsoft Graph Data Connect поддерживает извлечение данных из различных регионов Microsoft 365. Чтобы успешно переместить данные из центра обработки данных Microsoft 365 в хранилище Microsoft Azure, экземпляр фабрики данных Azure и расположение хранилища Azure должны сопоставляться с поддерживаемым регионом для расположения данных Microsoft 365. 

В следующей таблице указаны поддерживаемые регионы Microsoft 365 и соответствующие регионы Azure, необходимые для перемещения данных.

| Регион Office      | Регион Azure                                                   |
| ------------------ | ---------------------------------------------------------------|
| **Азиатско-Тихоокеанский регион**   | <ul><li>Восточная Азия</li><li>Юго-Восточная Азия</li></ul>             |
| **Австралия**      | <ul><li>Восток Австралии</li><li>Юго-восток Австралии</li></ul>   |
| **Европа**         | <ul><li>Северная Европа</li><li>Западная Европа</li></ul>             |
| **Северная Америка**  | <ul><li>Центральная часть США</li><li>Восточная часть США</li><li>Восточная часть США 2</li><li>Центрально-северная часть США</li><li>Центрально-южная часть США</li><li>Центрально-западная часть США</li><li>Западная часть США</li><li>Западная часть США 2</li></ul>                                            |
| **Соединенное Королевство** | <ul><li>Южная часть Соединенного Королевства</li><li>Западная часть Соединенного Королевства</li></ul>                     |

## <a name="sinks"></a>Приемники

Приемники — это выходное расположение, используемое фабрикой данных для размещения данных в хранилище Azure. Подключение к данным поддерживает следующие типы приемных хранилищ:

- [Azure Data Lake Storage 1-го поколения](/azure/data-lake-store/data-lake-store-overview)
- [Azure Data Lake Storage 2-го поколения](/azure/storage/blobs/data-lake-storage-introduction)
- [Azure Storage Blob](/azure/storage/blobs/storage-blobs-overview)

К приемникам применяются следующие характеристики:

- Выходные файлы имеют формат строк JSON. Формат вывода фиксированный, и его изменение не поддерживается. Однако вы можете использовать фабрику данных Azure, чтобы скопировать результат конвейера подключения данных в другой механизм хранения (например, базу данных SQL Azure).
- Проверка подлинности субъекта-службы является единственным поддерживаемым механизмом проверки подлинности для всех типов приемников при выполнении копирования с использованием Microsoft 365 в качестве источника.
- При использовании хранилища BLOB-объектов Azure в качестве приемника нужно убедиться, что у вашего приложения есть доступ участника данных хранилища BLOB-объектов к расположению хранилища BLOB-объектов Azure.

## <a name="see-also"></a>См. также

- [Соединитель фабрики данных Azure для данных Microsoft 365](/azure/data-factory/connector-office-365)
- [Политики и выставление счетов](data-connect-policies.md)
