# Global-Inventory-Order-Booking-Logic
// Global Product Engine
FUNCTION Manage_Inventory(Category) {
    IF Category == ("Robotics" OR "Hardware" OR "Missionary") {
        ALLOW Global_Order_Booking(ENABLED);
        SYNC Offline_Stock (Assam_Supermarket); // Real-time update
    }
}
